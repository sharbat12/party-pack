# Party Pack — Project Doc

Single-file party game collection. 22 game entries, 15 playable (luck games filtered out at load).

## Files
- `index.html` — everything: CSS, UI strings (EN/HE/ES/AR), all 22 game engines, PeerJS online layer
- `cover.svg` — logo/cover art (also the browser tab icon)
- `CHANGELOG.md` — what changed and when

## Run
- Open `index.html` in any modern browser (double-click works)
- Local play works fully offline after first load
- Online needs internet (PeerJS cloud + Google Fonts CDN)

## Architecture (keep it this way)
- **Screens**: one `.screen` div per view, `show(id)` switches. Game screens: `s-<game>`.
- **Flow**: language → games → mode/setup → intro → game → result. Tournament wraps multiple games.
- **State**: `players[]`, per-game state objects (`R,T,C,K,GU,RPS,DICE,...`), reset in each `startX()`.
- **Timers**: everything through `later()`/`every()` → cleared by `stopAll()`. Raw `setInterval` must self-terminate + check screen is active.
- **Scoring**: only via `addScore()` (fever multiplier + first-point achievement hook live there).
- **Online**: host is referee, star topology via PeerJS room `ppack3-CODE`. Guests never decide anything; every guest message is validated (round/turn/name match). Every wait has a timeout that auto-resolves.
- **i18n**: `STR[lang][key]`, `t()` with English fallback. RTL via `document.dir`. Never hardcode player-facing text.
- **Streaks** reset per game; **wins** persist per session; **names/lang/sound** persist in localStorage.

## Test checklist (no runner — use browser preview + console)
1. No console errors on load
2. Play one local game end-to-end (setup → result → other games)
3. Host + guest online round if possible
4. Skip button never strands anyone; timeouts always advance

## Gotchas
- No Node/Python here — verify by reading, not running
- `file://` blocks some APIs; PeerJS needs network
- `null > -1` is true — never use it as an emptiness check
- Guest state must survive host racing ahead (build fresh on every message)
- Template literals nest fine inside `${}` — keep them readable anyway
