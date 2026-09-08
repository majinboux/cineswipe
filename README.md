# 🎬 CineSwipe — Movie Discovery

> Swipe right on movies you want to watch. Swipe left on ones you don't. Your taste engine learns with every swipe.

**[▶️ Try it live →](https://majinboux.github.io/cineswipe/CineSwipe_v3_tmdb.html)**

---

## What It Does

CineSwipe is a Tinder-style movie discovery app. Swipe through movies, build a watchlist, and let the AI taste engine learn what you actually like. Connect a free TMDB API key and get real movie posters, live IMDb ratings, and actual streaming availability for Netflix, HBO Max, Disney+, Prime, Hulu, and 10 more services.

---

## Features

- 🎬 **Swipe deck** — drag physics, like / skip / super like, keyboard shortcuts
- 🎛️ **20+ filters** — genre, streaming service, decade, rating, runtime, MPAA, language, awards
- 🧠 **Taste engine** — learns your preferences, re-sorts the deck, shows match %
- 👤 **Multi-profile accounts** — up to 6 profiles, each with their own watchlist and taste data
- ✅ **Watched + ratings** — 5-star ratings, reactions, review text, date watched
- 📊 **Stats tab** — genre breakdown, platform preferences, watch history, taste title
- 👥 **Group mode** — 2-6 players take turns swiping, see what everyone agrees on
- 🔍 **Search** — live TMDB search, trending now, new releases
- 📱 **Mobile-first** — works great on iPhone and Android in the browser

---

## Quick Start

1. **[Open the live app](https://majinboux.github.io/cineswipe/CineSwipe_v3_tmdb.html)** in any browser
2. **Get a free TMDB API key** at [themoviedb.org/settings/api](https://www.themoviedb.org/settings/api) — takes 2 minutes
3. **Paste your key** when prompted → real posters and live data turn on instantly
4. **Start swiping** 🎬

> Works with AI-generated data even without a TMDB key.

---

## Streaming Services Supported

Netflix · HBO Max · Disney+ · Prime Video · Hulu · Peacock · Paramount+ · Apple TV+ · Showtime · AMC+ · Crunchyroll · Tubi · Pluto TV · Kanopy

---

## Files

| File | Description |
|------|-------------|
| `CineSwipe_v3_tmdb.html` | ✅ **Use this one** — real TMDB data, full features |
| `CineSwipe_v3.html` | AI-powered fallback, no API key needed |
| `CineSwipe_v2.html` | Earlier version — 64 embedded movies |
| `CineSwipe.html` | Original prototype |

---

## Also on This Repo

The `CineSwipe/` folder on Ryan's machine contains a full **FastAPI + React** production app:
- FastAPI backend, Motor/MongoDB, JWT auth, WebSockets
- React 18 + Vite frontend (1647 modules, clean build)
- 25 backend tests, all passing
- Couple Match Mode via live WebSocket
- AI chat via Qwen on OpenRouter
- Self-hosted SMTP for couple invites

---

## Stack

- Vanilla JS + HTML + CSS (prototype — zero build step)
- [TMDB API](https://www.themoviedb.org/documentation/api) — posters, ratings, streaming providers
- FastAPI + React 18 (full production app, local)

---

*Built by [Dancz Ministries](https://danczministries.com)*
