<div align="center">

# Ho Ngoc Thai

### Game Backend Developer

C#/.NET developer focused on backend game systems: player-state persistence, reward/economy logic, service APIs, Firebase/Photon integration, and production-ready data flows.

<p>
  <a href="https://github.com/HoNgocThaiGameDev?tab=repositories">
    <img src="https://img.shields.io/badge/GitHub-Repositories-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub repositories" />
  </a>
  <a href="#published-games">
    <img src="https://img.shields.io/badge/Published-Google_Play-34A853?style=for-the-badge&logo=googleplay&logoColor=white" alt="Published games" />
  </a>
  <a href="#selected-engineering-work">
    <img src="https://img.shields.io/badge/Focus-Game_Backend-512BD4?style=for-the-badge&logo=dotnet&logoColor=white" alt="Game Backend" />
  </a>
</p>

</div>

---

## What I Build

I build backend and service logic for games: reward flows, progression systems, save-state handling, API contracts, Firebase/Photon integrations, and internal tooling that makes game features easier to operate after release.

My current focus is backend reliability for game features: clear state transitions, defensive save migration, testable time logic, explicit edge-case handling, and behavior that QA can verify from a spec.

## Engineering Focus

| Area | Practical Ownership |
| --- | --- |
| Game services | Reward flow, progression rules, player eligibility, tracking hooks |
| Player data | Save data shape, migration, versioning, rollback-safe progress, persistence boundaries |
| Backend APIs | Service/API logic, admin/support flows, clean contracts between client and backend |
| Platform integration | Firebase, Photon, client/backend communication, runtime debugging |
| Quality | NUnit tests, reviewable code, edge-case coverage, production-risk thinking |

## Published Games

| Product | Platform | Demo | Focus |
| --- | --- | --- | --- |
| [Conveyer Craze: Card Sort](https://play.google.com/store/apps/details?id=com.NebulaSoftStudio.ConveyerCrazeCardSortPuzzle) | Google Play | [Video demo](https://drive.google.com/file/d/13uM9Clp1OSWHNPoUWi7ML1pGx7ZwWjDM/view?usp=sharing) | 3D conveyor card-sorting puzzle with level progression, coin economy, ads, and IAP |
| [Hyper Gunner Online](https://play.google.com/store/apps/details?id=com.DefaultCompany.HyperGunner) | Google Play | [Video demo](https://drive.google.com/file/d/1WqkOJWwkruTGs9fmKhWGQRR6GihPHoU0/view?usp=sharing) | Online bullet-hell action game with PVE, Coop/PVP, backend services, progression, ads, and IAP |

## Published Game Details

### Conveyer Craze: Card Sort

- **Gameplay:** 3D mobile card-sorting puzzle where each level generates colored card packs across multiple queue rows. The player taps the front pack of a row to send matching-color cards onto a spline-driven conveyor, then routes them into matching card boxes. A level is cleared when all queued cards, conveyor cards, deck cards, and active color counts are resolved.
- **Core systems:** Procedural conveyor layout selection, spawn-point filtering, dynamic card-pack generation, color-group balancing, start-box capacity limits, deck overflow retry logic, same-color group return from deck, card-box refill flow, win/retry panels, skip-level purchase, shuffle action, spin wheel, coin rewards, and persistent level/coin state.
- **Technology:** Unity 2022.3 LTS, C#, Unity Splines/SplineMesh for conveyor paths, DOTween/DOTween Pro for card movement and UI animation, Google Mobile Ads and Unity Ads for interstitial/rewarded ads, Unity IAP for coin purchases, PlayerPrefs for progression and currency persistence, TextMeshPro/UI, audio feedback, and Android vibration feedback.

### Hyper Gunner Online

- **Gameplay:** Online top-down bullet-hell/survivor-like action game where players select characters, enter PVE maps, survive monster waves, defeat bosses, gain EXP, and choose skill/stat perks during the run. The project also supports Coop/PVP flows with Photon Fusion sessions, including arena-style modes, battle royale mode data, team/player sync, kill feed, revive/death handling, and friend-based room joining.
- **Core systems:** Scene loading and character spawning, wave/boss gameplay loop, win-condition handling, perk and skill upgrades, player stats, inventory equipment, map rewards, quests, battle pass, daily/new-player rewards, shop/currency, leaderboard, mailbox, friends, presence, global messages, support/GM tools, local save, backend data export, analytics hooks, loading UI, localization, audio, event bus, and object pools for monsters, effects, drops, sounds, and damage popups.
- **Technology:** Unity 2022.3 LTS, C#, URP 14, Photon Fusion 2 Shared Mode, Firebase, Colyseus/WebSocket SQL backend option, VContainer dependency injection, UniTask async workflows, Unity Input System, Unity IAP, VoxelBusters AdsKit/AdMob, Google Play Games, TextMeshPro/UGUI, Newtonsoft JSON, PlayerSave/SecurePrefs persistence, ScriptableObject-driven content data, Jenkins, and Fastlane.

## Selected Engineering Work

| Project | Stack | What It Shows |
| --- | --- | --- |
| [Comeback Bonus Backend Logic Test](https://github.com/HoNgocThaiGameDev/comeback-bonus-liveops-test) | C#, .NET, NUnit | Backend-style event state machine, save migration, cooldown rules, reward flow, anti-cheat time boundaries, unit tests |
| [Hyper Gunner Online](https://github.com/HoNgocThaiGameDev/Hyper-Gunner) | Unity, C#, Photon Fusion, Firebase, VContainer | Published online action game with multiplayer, backend abstraction, player progression, economy, inventory, rewards, and mobile release experience |
| [Piano Tile Core Game Demo](https://github.com/HoNgocThaiGameDev/Piano-Tile-Core-Game-Demo) | Unity, C# | Core gameplay loop, input timing, game-state organization |
| [Protect Street Demo](https://github.com/HoNgocThaiGameDev/Protect_Street_Demo) | Unity, C# | Gameplay systems, project structure, combat/progression logic |
| [Shooter Defense](https://github.com/HoNgocThaiGameDev/Shooter-Defense) | Unity, C# | Shooter-defense gameplay logic and C# system organization |

## Technical Stack

| Category | Tools |
| --- | --- |
| Languages | C#, C++, JavaScript/TypeScript |
| Backend | .NET, ASP.NET Core, REST APIs, PostgreSQL |
| Game services | Photon, Firebase, Unity client integration |
| Testing | NUnit, unit-testable service logic, edge-case test design |
| Workflow | Git, GitHub, readable PR-style documentation, debugging from logs and repro steps |

## How I Approach Game Backend Systems

- Start from the PRD/spec and clarify ambiguous backend/service rules before coding.
- Keep configuration data separate from service/controller logic so rewards, cooldowns, and balance values can be tuned safely.
- Treat save state as production data: version it, migrate it, and avoid overwriting player progress.
- Use injectable time providers for testability and prepare production paths for trusted/server time.
- Write focused tests around edge cases: first-time user, rollback time, fast-forward time, cooldown boundaries, reward failure, and old-save migration.
- Prefer explicit event hooks for UI, Missions, analytics, and other systems instead of hidden coupling.

## Current Direction

I am strengthening my game backend skill set around service architecture, player-state persistence, reward systems, production debugging, API boundaries, Firebase/Photon integration, and reliable C# test coverage.

---

<p align="center">
  Open to Game Backend and C#/.NET game-service opportunities.
</p>
