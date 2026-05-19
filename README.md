# 🐛 IT Clicker v3.4.4

> The hilariously accurate idle clicker game for IT professionals. Build your bug empire, survive BSOD events, recruit legendary heroes, and prestige your way to digital godhood.

**[▶ Play Now on GitHub Pages](https://littlebeansf.github.io/it-clicker)**

---

## What Is It

An infinite idle clicker browser game — Cookie Clicker meets IT department. Click bugs, earn bugs, automate production with 69 buildings, recruit 20 heroes, and unlock 50 skins. All in a single self-contained HTML file. No install, no server, no dependencies.

---

## Current State — v3.4.4

| Feature | Count / Status |
|---|---|
| Buildings | **69** across 5 categories |
| Heroes | **20** (8 IT memes + 12 named) |
| Skins | **50** (30 + 20 premium) |
| Upgrades | **151** (2 per building + click/prestige upgrades) |
| Achievements | **420** across 14 categories |
| Mini-games | **4** (Bug Catcher · Sirtet.exe · git_snake.exe · BSOD Clicker) |
| Prestige system | ✅ Escalating thresholds, CPU Core multipliers |
| Offline earnings | ✅ Up to 8h, 50% efficiency, modal on return |
| Anti-cheat | ✅ Autoclicker detection, escalating lockouts |
| Sound / Music | ✅ 3 background tracks + ambient SFX |
| Mobile | ✅ Mobile-first responsive layout |
| Dark / Light mode | ✅ |
| Admin mode | ✅ Click the ⓘ button 69 times |
| Save system | ✅ HMAC-SHA256 signed export/import |

---

## Buildings — 5 Categories

| Category | Count | Examples |
|---|---|---|
| **Junior Dev Zone** | 13 | Rubber Duck, Coffee Machine, Intern, Git Repo, Jira Board |
| **Infra Layer** | 14 | Server Rack, Cloud VM, Load Balancer, Kubernetes, CI/CD Pipeline |
| **People Layer** | 14 | Scrum Master, Open Office, HR Portal, Hackathon, Bug Bounty |
| **Advanced Systems** | 13 | AI Assistant, Blockchain Node, Quantum Computer, Docker Swarm |
| **Cosmic Tier** | 15 | Bug Singularity, Dark Matter Farm, Void Compiler, Warp Drive, Omniscient AI |

All 69 buildings have unique **128×128 pixel art** (isometric 16-bit style, dark backgrounds, neon glow).

---

## Heroes — 20 Total

### IT Meme Heroes (1–8)
| Hero | Reference | Bonus |
|---|---|---|
| Linus the Kernel | Linus Torvalds | All categories +25% |
| Jon Skeet | Stack Overflow legend | Click power +30% |
| This Is Fine | Burning room dog | Junior +40% |
| Stallman the GNU | Richard Stallman | Infra +40% |
| Agile Coach Karen | "Let's synergize the sprint" | People +35% |
| The 10x Dev | "Rewrote it in Rust" | Advanced +35% |
| Sudo Sam | `sudo make me a sandwich` | Advanced +50% |
| Segfault Sally | Core dumped, reality crashed | Cosmic +60% |

### Named Heroes (9–20)
| Hero | Bonus |
|---|---|
| Sebi the Creator | All +30% |
| Dome the Big D | Advanced +45% |
| Gaya the PM | People +45% |
| Nik the Marketer | Junior +50% |
| Ladinsch with the Money | Infra +50% |
| Mic the Brain | Advanced +55% |
| Pepe the Coder | Junior +35% |
| Anonymous Hacker | Cosmic +65% |
| Jan the Gamer | Click +30% |
| Mel the Rasta | All +20% |
| Elia the Intern | Junior +45% |
| Paddl 67 | Advanced +40% |

Heroes unlock after your **first prestige**. Each has a unique 128×128 isometric pixel art portrait.

---

## Mini-Games

| Game | Description |
|---|---|
| **Bug Catcher** | Tap falling bugs before they escape — earn bonus clicks |
| **Sirtet.exe** | Tetris with a twist — stackable bug blocks |
| **git_snake.exe** | Classic snake with arrows — eat commits |
| **BSOD Clicker** | Survival drain bar — click to keep the system alive during a BSOD event. Easy / Hard / PANIC difficulties. Rewards based on performance. |

---

## Prestige System

- Threshold: `1e12 × 1.5^prestige_count` — genuinely hard to reach
- Reward: CPU Core multipliers (capped at 30 total)
- Cores per prestige: `min(3, floor(√(runBugs / 1e12)))`
- BSOD winnings are capped to prevent exploit-based fast prestige
- Heroes unlock on **first prestige only**

---

## Offline Earnings

When you return after ≥1 minute away, a "Welcome Back" modal shows:
- Time away (formatted: seconds / minutes / hours)
- Bugs earned at **50% efficiency** while offline
- Progress bar showing % of 8h cap used
- One-tap **Collect** button to apply earnings

---

## Anti-Cheat

- CPS monitoring — threshold: >20 clicks/sec
- Escalating lockouts: 30s → 60s → 120s
- HMAC-SHA256 signed save exports — tampered saves rejected on import

---

## Performance

All pixel art: generated at 512×512+ PNG → compressed to **128×128 WebP quality 75**.
- Total image payload: ~0.2 MB for all 89 images (69 buildings + 20 heroes)
- Zero external dependencies — game is a **single 5.3 MB HTML file**
- Canvas-based mini-games pause when not in view
- RequestAnimationFrame loop with delta-time capping

---

## Tech Stack

- Pure **HTML / CSS / JavaScript** — no build step, no framework, no server
- Web Audio API — all SFX procedural, background music via AudioContext
- Canvas API — mini-games, particle system, background animation
- SubtleCrypto API — HMAC-SHA256 for save signing
- WebP pixel art — 128×128, quality 75, method 6 (Pillow/libwebp)
- GitHub Pages for hosting

---

## Save Key

`itclicker_v2_save` — localStorage. Includes: bugs, totalBugs, runBugs, allTimeBugs, buildings, upgrades, achievements, heroes, prestige count, cores, skin, music settings, lastSave timestamp.

---

*"It works on my machine."* — Every developer, forever
