# BashProject-SSOOI

Bash implementation of **Cinquillo** (5illo), a Spanish card game where players take turns placing cards adjacent to the 5s on the table. Features two AI difficulty levels with different playing strategies.

Built as a team project for the **Sistemas Operativos I (SSOOI)** course.

## How it works

The game follows standard Cinquillo rules: the player who holds the 5 of coins starts, and players take turns placing cards that are adjacent (in rank) to cards already on the table. If you can't play, you pass. The first player to empty their hand wins.

The AI opponent has two strategies:

- **Easy mode** — Plays cards matching suits already on the table. Falls back to playing a 5 if no match is found.
- **Hard mode** — Analyzes its hand strategically:
  - Plays a 5 if it also holds the 1, 9, or 10 of that suit (maximizing future plays)
  - Plays a 5 of the suit where it has the most cards
  - Otherwise, avoids playing 5s to keep options open

## Running it

```bash
chmod +x 5illo.sh
./5illo.sh
```

Configuration is loaded from `config.cfg` and game logs are written to `fichero.log`.

## Tech stack

| | |
|---|---|
| **Language** | Bash |
| **Platform** | Linux |

## Context

Built for the **Sistemas Operativos I (SSOOI)** course at Universidad de Salamanca, 2023. The project exercises Bash scripting fundamentals: control flow, string manipulation, file I/O, and game logic.
