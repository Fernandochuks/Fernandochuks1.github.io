# Fernandochuks1.github.io
NEON
# NEON EMPIRE — Strategic City, Business & Tri-Theater Warfare Game

A full-stack strategic empire simulation built for Telegram Mini Apps (`window.Telegram.WebApp`) and the Telegram Gaming Platform (`setGameScore`).

## Core Pillars of NEON EMPIRE

1. **Everyday Human Life & City Development**:
   - Charter housing arcologies, commuter transit lines, hospitals, and universities to grow your **Citizen Population** and **Morale (%)**.
2. **Commercial Businesses & GDP Economy**:
   - Operate FinTech exchanges, retail megamalls, deepwater cargo terminals, and aerospace plants to generate per-turn **Treasury Credits ($k)**.
3. **Tri-Theater Warfare (Air, Land & Sea)**:
   - Command **Air Force Wings (Air)** across Row A–B high-rise skyports, **Armored Mechanized Divisions (Land)** across Row C–D urban/industrial corridors, and **Naval Carrier Fleets (Sea)** across Row E deepwater harbors.

## Architecture

- `client/src/main.tsx` — Telegram WebApp frontend with Empire Map, City & Businesses tab, Tasks tab, and Alliances tab.
- `server/src/index.ts` — Express server verifying `Telegram.WebApp.initData` via HMAC-SHA256, processing business upgrades, and syncing `setGameScore`.
- `server/db/schema.sql` — SQL schema storing `empires`, `city_businesses`, `war_campaigns`, `alliances`, and `empire_tasks`.

