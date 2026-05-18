# 🐛 IT Clicker v3.4

> The hilariously accurate idle clicker game for IT professionals. Build your bug empire, survive BSOD events, unlock legendary heroes, and prestige your way to digital godhood.

**[▶ Play Now on GitHub Pages](https://littlebeansf.github.io/it-clicker)**

---

## What's New in v3.4

### 69 Buildings — 5 Categories
Buildings are now organized into five tiers with category-specific hero bonuses:

| Category | Buildings |
|---|---|
| **Junior** | Rubber Duck, Coffee Machine, Sticky Note, Whiteboard, Rubber Duck Farm, Intern, Help Desk, Git Repo, Slack Channel, Meetup, Docs Site, Bug Report, Code Review |
| **Infra** | Server Rack, Cloud VM, Load Balancer, Firewall, Backup Server, VPN, Database Cluster, API Gateway, Monitoring Stack, Microservices, CI/CD Pipeline |
| **People** | Open Office, Meeting Room, Scrum Master, HR Portal, Hackathon, Open Source Project, Bug Bounty, Conference, Startup Incubator, Auto Tests |
| **Advanced** | Data Center, AI Assistant, Blockchain Node, Quantum Computer, Docker Swarm, Feature Flags, Serverless Functions, Penetration Tester |
| **Cosmic** | Bug Singularity, Dark Matter Farm, Quantum Entangler, Void Compiler, Warp Drive, Singularity Core, Black Hole Server, Omniscient AI |

All 69 buildings have unique **128×128 pixel art** (isometric 16-bit style, dark backgrounds with glow effects).

### 189+ Upgrades — 2 Per Building
Every building has exactly 2 upgrades that visually reflect on the building icon when purchased. Upgrades scale progressively and are sorted by affordability.

### 16 Heroes — Named + IT Meme Characters

| Hero | Bonus |
|---|---|
| **Paddl67** | All categories +20% |
| **Jan the Architect** | Advanced +40% |
| **LittleBean** | All categories +25% |
| **The PM** | People +40% |
| **Big D** | Infra +35% |
| **Root** | Infra +45% |
| **Quantum** | Cosmic +60% |
| **Sebi the Creator** | All categories +30% |
| **Dome the Big D** | Advanced +45% |
| **Gaya the PM** | People +45% |
| **Nik the Marketer** | Junior +50% |
| **Ladinsch with the Money** | Infra +50% |
| **Mic the Brain** | Advanced +55% |
| **Pepe the Coder** | Junior +35% |
| **Anonymous Hacker** | Cosmic +65% |
| **The DBA** | Infra +30% |

Heroes are recruited after your **first prestige** and each has a unique pixel art portrait.

### 50 Skins
Unlock custom click button skins as you progress. All skins are pixel art WebP at 128×128, compressed for maximum performance:

Matrix, Hackerman, Retro Terminal, Cyberpunk, Win XP, Synthwave, Space Station, Vaporwave, Deep Sea, Steampunk, Lava Lamp, Neon Zen, Minecraft, Bitcoin Bull, Dungeon, Arctic, Nuclear, Corporate, Y2K, Doomscroll — plus 30 more.

### BSOD Event — Redesigned
- **No more confusion** — bouncing `▼ CLICK HERE ▼` arrow clearly shows the click target
- **Alarm phase** triggers falling-code rain immediately when the countdown hits zero
- **Easy difficulty rebalanced** — slower AI, smaller stake, longer timer
- **Result panel** auto-scrolls into view after each round
- **Text-only phase indicators** (`!` / `!!` / `!!!`) — no emoji clutter
- Exploit-proof: BSOD winnings are capped so it cannot be abused for fast prestige

### Anti-Cheat System
- Autoclicker detection (>20 CPS threshold)
- Escalating lockouts: 30s → 60s → 120s
- HMAC-SHA256 signed save exports — tampered saves are rejected on import

---

## Full Feature List

- 🏢 **69 buildings** across 5 categories (Junior / Infra / People / Advanced / Cosmic)
- 🦸 **16 heroes** with category-specific bonuses — unlocked after first prestige
- 🎨 **50 skins** for the click button — all compressed pixel art WebP
- ⬆️ **189+ upgrades** — 2 per building, visually applied to building icons
- 🏆 **420 achievements** across 6 categories
- 🎮 **5 mini-games**: Bug Catcher, Sirtet.exe, Oldschool Snake, BSOD Clicker, Memory Leak
- 🔄 **Prestige system** — resets progress for permanent CPU Core multipliers; heroes unlock on first prestige
- ⚡ **Combo system** — up to ×50 multiplier with fever mode; 100% combo triggers a bug explosion animation
- 📻 **3 background music tracks** — Patch Day Loop (slow) / Scrum Glitch (medium) / Scrum Loop (fast); autoplay from settings
- 🔊 **Sound system** — ambient sounds + SFX, all controls in settings
- 🌓 **Light / Dark mode**
- 📱 **Mobile-first** — fully playable on phones and tablets
- 🔒 **Signed save export/import** — HMAC-SHA256, tamper-proof
- 🛡️ **Anti-cheat** — autoclicker detection with escalating lockouts
- 🔧 **Admin mode** — click the ⓘ button in Settings 69 times
- 📴 **Single HTML file** — zero dependencies, works offline

---

## Tech Stack

- Pure HTML / CSS / JavaScript — no build step, no framework
- Web Audio API for all sound (no external audio files for SFX)
- Canvas API for mini-games
- WebP pixel art assets (128×128, ~0.18 MB total for all 75 images)
- HMAC-SHA256 via SubtleCrypto API for save signing

---

## Performance

All pixel art assets were generated at 512×512+ PNG and compressed down to 128×128 WebP at quality 75 — **99.8% size reduction** (113 MB → 0.18 MB). The game is designed to remain fluid even with all 69 buildings purchased and multiple mini-games running simultaneously.

---

## Prestige & Progression

Progression is intentionally slow — you need to genuinely grind to reach prestige. The BSOD event reward cap and anti-cheat system prevent exploit-based skipping. After each prestige you earn a CPU Core multiplier and unlock the hero roster.

---

*"It works on my machine."* — Every developer, forever
