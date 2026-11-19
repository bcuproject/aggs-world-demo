# A.G.G's Restaurant & Bar — interactive demo website

Live demo: https://bcuproject.github.io/aggs-world-demo/
Mobile preview (phone frame + QR code): https://bcuproject.github.io/aggs-world-demo/mobile.html

A single-page demo site for A.G.G's (African Nigerian cuisine, Coventry & Leicester).

## Features
- **Menu** with animated dish illustrations, heat filter, search and a build-your-own-plate tool
- **Pop-up ordering**: basket, pick-up details, demo order placement with a live order tracker, or send via WhatsApp
- **Naija News**: live Nigerian headlines (Premium Times, Punch, Vanguard), illustrated covers, read-aloud, save and share, GBP→NGN converter, Lagos clock
- **Jollof Rush** arcade game with synthesised sound effects and music, plus a food trivia quiz and leaderboard
- **Our Story** animated story player and highlight clips
- **Chat assistant** for hours, locations, prices, order tracking and WhatsApp hand-off
- **Mobile-first**: app-style bottom tab bar, two-column menu, portrait game, swipeable story, haptics, installable to the home screen (web app manifest + icons)
- Live open/closed status and countdown, dark/light mode

## Demo data
Prices, demo orders, highlight clips, leaderboard scores and the fallback exchange rate are **sample data** for demonstration.
Edit the `PRICES`, `DISHES` and `VIDEOS` lists near the top of the `<script>` in `index.html` to use real content.

## Releasing an update
The installed app checks `version.json` for new releases (on open, when brought back to the foreground, every 5 minutes and when back online) and offers a one-tap update.
When publishing a change, bump the version in **three** places so phones are told about it:
1. `APP_VERSION` / `APP_UPDATED` at the top of the `<script>` in `index.html`
2. `version` (and the one-line `notes`) in `version.json`
3. `CACHE` in `sw.js`
