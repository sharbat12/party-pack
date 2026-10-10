# Party Pack — Roadmap

## Done
- [x] 15 skill games (luck games removed, poker kept)
- [x] Local 2–8 + online rooms (host referees, timeouts everywhere)
- [x] 4 languages + RTL, mouse-first + per-keyboard-keys
- [x] Combos, 8 achievements, fever rounds, session win crowns
- [x] Tournament mode, filters, skill section, surprise, sound toggle
- [x] Skins (avatar picker), mature theme, SVG icons, cover art
- [x] Juice: shake, particles, floating scores, typewriter, stagger
- [x] 🔥 HARD mode toggle (persisted): faster reaction + fakes, 8s country timer, earlier hard trivia, 4s clicker, faster bullseye, earlier balloon pops, 4-miss hangman, +3 simon growth, 12s trivia timeout
- [x] Online hub (pick/surprise → lobby), duplicate-name fix, reconnect guards
- [x] Offline fallback message when PeerJS can't load

## Next (ordered)
1. [ ] More achievements (per-game feats: poker royal exists; add memory perfect, typing sub-10s)
2. [ ] Team mode (2v2 / boys-vs-girls scoring)
3. [ ] Daily challenge seed (same trivia order for everyone, one day)
4. [ ] Sound effects upgrade (WebAudio melodies per game, not just beeps)
5. [ ] New games only if skill-based: archery wind, code-breaker (Mastermind), chess-clock blitz quiz
6. [ ] PWA manifest so phones can install it (needs hosting — won't work on file://)
7. [ ] Reconnect mid-game (currently a refresh = rejoin as new player)

## Never
- Luck-only games (slots, pure dice, lottery) — poker stays, it's skill
- Accounts, servers, or databases — peer-to-peer only
- Breaking the one-file build (`index.html` + `cover.svg` only)
