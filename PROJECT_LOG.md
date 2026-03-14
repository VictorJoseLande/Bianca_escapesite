# Project Log: The Story of Bianca — Escape Site

## Overview

A birthday gift for Bianca: a 10-level interactive "escape room" webpage themed as the epic (and ridiculous) tale of a Croatian princess fleeing to Norway. Built and deployed in under 30 minutes on 2026-03-14.

**Live URL:** https://victorjoselande.github.io/Bianca_escapesite/
**Repository:** https://github.com/VictorJoseLande/Bianca_escapesite

---

## Concept

- **Theme:** "A Croatian princess running away from her kingdom to the vikingland of Norway and finding her light"
- **Recipient:** Bianca — a Croatian friend living in Norway. Known for being loud, kind, creative, fashionable, a party lover, espresso addict, periodic diva, and the best listener in every room.
- **Tone:** Over-the-top fairy tale narrator voice. Simple, ironic, and very funny. The humor comes from exaggerating Bianca's real-life journey into an absurd epic.

---

## Tech Stack

- **Single HTML file** (`index.html`) — no framework, no build step, no dependencies
- **Embedded CSS + JavaScript** — everything self-contained
- **Fonts:** Google Fonts (Cinzel Decorative, Lora, Inter)
- **Hosting:** GitHub Pages (free, permanent, instant deploy)

### Why this approach?
Speed. With a 30-minute deadline, a single HTML file with GitHub Pages was the fastest path from idea to live URL. No npm, no React, no build pipeline.

---

## Story Arc — 10 Levels

| Level | Title | Story Beat | Puzzle Type |
|-------|-------|-----------|-------------|
| 1 | The Last Espresso | The kingdom runs out of espresso. National emergency. | Unscramble "ESPRESSO" |
| 2 | The Royal Wardrobe Crisis | Can't flee without the right diva escape outfit. | Multiple choice (pick the outfit) |
| 3 | Sneaking Past the Guards | Distracts the guards with a murder mystery party. | Multiple choice (party type) |
| 4 | The Adriatic Sea Crossing | Steals a yacht; navigation locked behind Croatian trivia. | Multiple choice (capital of Croatia) |
| 5 | The European Detour | Accidentally ends up inside an IKEA in Sweden. | Text input (IKEA furniture pattern) |
| 6 | The Viking Greeting | Culture shock — Norwegians stand 3 meters apart. | Matching puzzle (customs to meanings) |
| 7 | The Great Darkness | Norwegian winter. The sun disappears for months. | Riddle (answer: the sun) |
| 8 | The Party Revival | Bianca throws a murder mystery and makes Norwegians loud. | Multiple choice (solve the mystery) |
| 9 | The Friends She Made | Everyone loves her — she's the loudest and kindest. | Multiple choice (her true superpower) |
| 10 | Finding Her Light | The sun returns, but the real light was Bianca all along. | Text input (answer: birthday) |

### Post-Level 10: Two-Stage Finale

1. **Birthday message screen** — heartfelt message with confetti, "OUF!", and the reveal that "You ARE the light, Bianca"
2. **Gift card reveal** — "But wait... claim your prize!" button leads to the Squeeze massage gift card with dramatic animations

---

## Visual Design

- **Color palette:** Dark purple/black background, gold accents, cream text
- **Background:** Animated starfield with twinkling stars
- **Fonts:** Cinzel Decorative for titles (royal/fairy tale feel), Lora for story text, Inter for UI elements
- **Progress bar:** Gold gradient bar at the top, fills as levels are completed

### Animations
- **Twinkling stars** — random positioned, varied timing
- **Floating emojis** — level icons bob up and down
- **"OUF!" pulse** — text scales up and down for emphasis
- **Running princess** — `👸💨` runs across the screen between levels
- **Correct/wrong feedback** — green pulse for correct, red shake for wrong
- **Confetti** — 60 multicolored pieces rain down on the finale
- **Gift card reveal** — 3D flip animation with golden shimmer border
- **Sparkles** — floating emoji sparkles during gift reveal
- **Shimmer border** — animated gradient border around the gift card

---

## Puzzle Types Implemented

1. **Unscramble** — click letters to build a word, with clear/reset
2. **Multiple choice** — 4 options in a grid, visual correct/wrong feedback
3. **Text input** — type answer, accepts multiple valid answers (e.g., "SUN", "SOL", "SOLEN")
4. **Matching** — click left item then right item to pair them
5. **Riddle** — riddle text + text input for the answer

---

## Features (added post-launch)

### Progress Saving
- Current level saved to `localStorage` on every navigation action
- Refreshing the page resumes at the exact level/page you were on
- "Play Again" button clears saved progress

### Secret Password Fast-Track
- Password field on the title screen (subtle, below the start button)
- Entering `OUF2026` skips directly to the gift card reward page
- Password is only revealed at the bottom of the reward page after completing the quest

### Back Button Navigation
- "Go Back" button appears at the top of every chapter
- Chapter 1 goes back to the title screen
- Going back saves progress so refreshing stays on the current page

### Feedback Fix
- When selecting the correct answer, the response message and the success message are shown stacked (appended), not replacing each other
- Prevents the jarring experience of text being yanked away mid-read

---

## Files

| File | Purpose |
|------|---------|
| `index.html` | The entire escape site — HTML, CSS, and JS |
| `giftcard.pdf` | Squeeze massage gift card (the prize) |
| `PROJECT_LOG.md` | This file |

---

## Git History

| Commit | Description |
|--------|-------------|
| `9c50f9e` | Initial build — all 10 levels, animations, puzzles, birthday finale |
| `0ecc8d0` | Added gift card reveal as final prize with shimmer/sparkle animations |
| `c354a2d` | Added project log |
| `47c9019` | Added progress saving, secret password (OUF2026), back button on all levels, and feedback append fix |

---

## Deployment

1. Repository created on GitHub: `VictorJoseLande/Bianca_escapesite`
2. GitHub Pages enabled — source: `main` branch, root folder
3. Site live at: https://victorjoselande.github.io/Bianca_escapesite/
4. Hosting is free and permanent (until repo is deleted or Pages disabled)

---

## Personal Details Woven Into the Story

- "OUF!" — Bianca's signature exclamation, used throughout
- Espresso + cigarettes on a Croatian summer day — the inciting incident
- Periodic diva energy — the wardrobe crisis level
- Murder mystery creator — she literally invented one for friends (level 3 and 8)
- Loudest person in every room — referenced multiple times, turned into a superpower
- Amazing listener — the paradox of being loud AND the best listener
- Stylish and fashionable — the escape outfit puzzle
- People lover — the friends-she-made level
- Party era — the party revival level
- Typical Croatian — Croatian trivia and cultural references
- Positive and kind — the emotional core of the story

---

## Process

1. Brainstormed the concept collaboratively (clarifying questions about Bianca, puzzle preferences, tech-savviness)
2. Agreed on single-HTML-file + GitHub Pages for maximum speed
3. Designed the 10-level story arc with increasing difficulty
4. Built the entire site in one file write
5. Deployed via GitHub Pages
6. Added gift card reveal as the final prize
7. Total time: under 30 minutes from idea to live URL
8. Post-launch: added progress saving, secret password, back button, and feedback fix (ported from Rafal's escape site improvements)
