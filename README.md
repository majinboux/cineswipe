# CineSwipe

A movie recommendation app. Swipe right to like, left to pass, until you land on something to watch tonight. Couple mode finds movies both of you want.

## What is real now

Built with FastAPI (Python) backend and React/Vite frontend. Working as of 2026-08-22.

- Swipe UI with a 40-film curated local library across 12 genres and 10 moods
- Genre and mood filtering, plus a streaming-service filter
- Match overlay on every right swipe
- Movie detail sheet with synopsis, runtime, genres, moods, streaming tags
- JWT auth (bcrypt), watch history, watchlist, couple linking via invite
- Couple Match Mode (Tonight's Pick): both linked accounts swipe right on the same film and the match fires over a live WebSocket -- verified end-to-end with real accounts
- AI chat wired to Qwen 3.7 Flash via OpenRouter (thinking mode disabled -- had to fix that)
- Couple invite email via R510 self-hosted SMTP relay
- 25 backend tests, all passing (no MongoDB or API key required)
- `npm run build` clean: 1647 modules, no errors

## Stack

| Layer | What |
|---|---|
| Backend | FastAPI, Python 3.11, Motor/MongoDB, JWT/bcrypt, WebSockets |
| Frontend | React 18, Vite, Tailwind CSS, shadcn/ui-style primitives |
| AI chat | OpenRouter -- `qwen/qwen3.7-flash` |
| Email | Self-hosted SMTP relay |
| Tests | pytest, 25 tests |

## Structure

```
CineSwipe/
  backend/
    server.py           FastAPI entry -- all routes + middleware
    movie_service.py    Filtering, TMDB/OMDb integration (inactive without keys)
    movies_data.py      40-film curated local library
    models.py           Pydantic models
    auth.py             JWT + bcrypt
    database.py         Motor/MongoDB connection
    ai_chat_service.py  OpenRouter Qwen chat
    email_service.py    SMTP invite email
    tests/              25 passing tests
  frontend/
    src/
      pages/            SwipePage, AuthPage, HistoryPage, SettingsPage, WatchlistPage
      components/       SwipeCard, MatchOverlay, MovieDetailSheet, AIChatSheet, BottomNav
      context/          AuthContext
      hooks/            useSwipeGesture, useApiData
      lib/              api client, utils
      constants/        genres, moods, streaming services
```

## Run it

```bash
cd backend
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
copy .env.example .env
python -m uvicorn server:app --host 0.0.0.0 --port 8001 --reload
```

```bash
cd frontend
npm install
copy .env.example .env
npm run dev
```

Frontend at `http://localhost:3000`. Backend health: `http://localhost:8001/api/health`.

Tests (no MongoDB or API key needed):
```bash
cd backend && pytest
```

## What still needs work

- TMDB and OMDb API keys to pull live movie data (hooks are wired, inactive without keys)
- MongoDB for auth, history, watchlist, couple linking (app serves local library without it)
- Streaming availability is representative data, not live-verified per title
- No real poster art without a TMDB image key (gradient placeholder is shown instead)
- Store submission

## Source

`C:\Users\ryand\OneDrive\CineSwipe` on Ryan's machine. Part of Dancz Ministries LLC.