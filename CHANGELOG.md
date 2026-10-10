# Party Pack — Changelog

One file: `index.html` (+ `cover.svg`). Everything below lives in it.

## v5.6 — Typo forgiveness (current)
- Country accepts close spellings (ISRAL → ISRAEL): 1 typo allowed up to 7 letters, 2 for longer, exact only for short names, first letter must match

## v5.5 — HARD mode (current)
- 🔥 toggle on games screen (saved): faster reaction + more fakes, 8s country timer, hard trivia from round 3/2, 4s clicker, faster bullseye, earlier balloon pops, 4-miss hangman, +3 simon growth, 12s online timeouts

## v5.4 — Online hub + fixes
- Online section: pick a game or Surprise, then lobby; loops back after matches
- Fixed: duplicate nicknames broke turn detection, double Create/Join/Start, stale peers, bingo tally 6s

## v5.3 — Realism in game pieces
- Vector dice, geometric memory, growing balloon + burst, RPS tiles, bingo balls, film grain

## v5.2 — Juice system
- Screen shake, particle bursts, floating scores, staggered cards, typewriter titles

## v5.1 — Harder difficulty
- Reaction windows, big math, simon +2, 5-miss hangman, faster aim, earlier pops, 5-word typing

## v5.0 — 5 skill games (20 entries)
- Bullseye, Math Duel, Type Race, Sequence, Scramble

## v5.0 — Realism pass (current)
- Vector dice with real pips + roll animation (was unicode faces)
- Memory pairs are geometric shapes with gold card backs (was fruit emojis)
- Vector balloon that grows while held + gold burst on pop
- RPS redesigned as rock/paper/scissors vector tiles
- War cards, bingo-ball cage display, gauge ticks, beveled Simon pads, glowing signal lamp, film grain

## v4.9 — 2 skill games + wins (22 entries)
- New: Stroop (tap the ink, not the word), Odd One Out (spot the different dot)
- Session wins counter (crowns on score chips)
- Royal Flush achievement (straight flush in poker)
- 22 games total

## v4.8 — Juice system
- Screen shake, gravity particle bursts, floating score text, staggered cards, typewriter titles
- Single shared FX module (canvas only runs while particles exist)

## v4.7 — Harder (9th grade)
- Faster reaction windows, bigger math numbers, Simon +2/round, 5-miss hangman, faster bullseye, earlier balloon pops
- Poker rules text restored to full rules

## v4.6 — Online section + online fixes
- Online hub: pick a game or Surprise, then lobby
- Fixed: duplicate nicknames broke turn detection (host confirms final name)
- Fixed: double Create/Join/Start, stale connections destroyed, bingo tally 6s

## v4.5 — Shared-screen secrets
- Poker: cards never shown openly local — hold-to-peek only
- RPS: turn-based picking in random order + look-away

## v4.4 — Luck purge (15 playable)
- Removed from play: balloon, dice, war, bingo, number guess, RPS, hi-lo (pure luck; poker stays for skill)
- 22 entries in code, 15 playable: reaction, trivia, country, clicker, poker, simon, hangman, memory, aim, math, type, seq, scramble, stroop, oddone

## v4.3 — Combos, achievements, fever
- Streaks with 🔥 flames, +1 bonus every 3rd consecutive success
- 7 achievements + toasts (First Blood → Champion)
- 25% Fever rounds (double points, synced online)

## v4.2 — Tournament + memory
- Tournament mode (pick 2–5 games, totals, podium), local only
- Saved language + names, game filters, sound toggle, surprise button

## v4.1 — 5 more skill games (20 total)
- Bullseye, Math Duel, Type Race, Sequence, Scramble

## v4.0 — Poker + 4 games (15 total)
- Poker Night: 100 chips, ante, 3 streets, full hand evaluator, online private hole cards

## v3.x — Foundations
- 10 games, 4 languages (EN/HE/ES/AR, RTL), mouse-first + per-player keys
- Trivia elimination with easy/med/hard tiers
- Local 2–8 + online PeerJS rooms, host-authoritative protocol
- Skins (avatar picker), mature theme, SVG icons, cover art
- Tournament, filters, combos came later (see above)

## Rules worth remembering
- Luck games stay out (poker is the exception — it has skill)
- Every game: local + online, mouse-first, 4 languages
- Host is always the referee online; timeouts everywhere so games never stall
- Scores reset per game; streaks reset per game; wins persist per session
