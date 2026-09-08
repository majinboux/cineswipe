#  CineSwipe
### Swipe-Based Movie Discovery App  Dancz Ministries LLC

> Swipe right on movies you want to watch. Swipe left on ones you don't. Let your taste build itself.
>
> CineSwipe is a swipe-based movie and TV discovery app that learns your taste through your swipes and builds a personalized watchlist automatically  no search, no scrolling, no decision fatigue. Platform-agnostic across Netflix, Hulu, Prime, Max, Disney+, and Apple TV+.
>
> ---
>
> ##  The Problem
>
> 85M+ US streaming subscribers. Every one of them opens an app, scrolls for 20 minutes, and watches nothing. Decision fatigue is a real, documented phenomenon  and every streaming platform makes it worse. CineSwipe solves it with one mechanic: swipe.
>
> ---
>
> ##  Core Features
>
> - **Swipe-to-discover**  movie poster, title, year, rating, one-line hook. Decide in under 2 seconds
> - - **Taste engine**  learns genre, director, decade, tone from your swipe history. Gets better every session
>   - - **Watchlist**  auto-organized by streaming platform so you know exactly where to watch
>     - - **Group mode**  swipe with your partner or family. CineSwipe finds the overlap
>       - - **Watch Now**  deep links directly into the streaming app
>         - - **Mood filter**  funny / scary / short / feel-good pre-filters the deck
>          
>           - ---
>
> ##  Business Model
>
> | Stream | Details |
> |--------|---------|
> | Freemium | Free: 20 swipes/day, basic watchlist |
> | Premium $3.99/mo | Unlimited swipes, group mode, mood filters, offline watchlist |
> | Affiliate | Commission from streaming referrals (Apple, Amazon affiliate programs) |
> | Promoted Titles | Studios pay to surface new releases in the swipe deck |
>
> ---
>
> ##  Tech Stack
>
> | Layer | Tech |
> |-------|------|
> | Mobile | React Native (iOS + Android) |
> | Movie Data | TMDB API  500k+ titles with posters |
> | Streaming | Watchmode API  real-time availability by platform |
> | Backend | Supabase (Postgres + Auth + Storage) |
> | Taste Algorithm | Collaborative filtering on swipe history |
> | Deep Links | Universal Links (iOS) + App Links (Android) |
>
> ---
>
> ##  What's in This Repo
>
> | File | Description |
> |------|-------------|
> | `docs/CineSwipe_Project_Summary.docx` | Full project summary  concept, market, tech, monetization |
>
> ---
>
> ##  Roadmap
>
> - [ ] TMDB API integration for movie card data
> - [ ] - [ ] Swipe UI  React Native Animated + Gesture Handler
> - [ ] - [ ] Taste engine  genre/director/decade weighting
> - [ ] - [ ] Streaming availability lookup via Watchmode
> - [ ] - [ ] Watchlist organized by platform
> - [ ] - [ ] Group swipe mode with real-time match detection
> - [ ] - [ ] Mood filter UI
> - [ ] - [ ] App Store + Google Play submission
>
> - [ ] ---
>
> - [ ] ##  Links
>
> - [ ] - **Dancz Ministries**  [danczministries.com](https://danczministries.com)
> - [ ] - **All Projects**  [dancz-projects](https://github.com/majinboux/dancz-projects)
> - [ ] - **Contact**  ryan@danczministries.com
>
> - [ ] ---
>
> - [ ] *Built by Ryan Dancz  100% P&T disabled veteran, founder Dancz Ministries LLC, Lugoff SC.*
