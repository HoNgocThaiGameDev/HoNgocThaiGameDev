<div align="center">

# Ho Ngoc Thai

### Game Backend / Unity LiveOps Developer

C#/.NET developer focused on game systems, player-state persistence, reward logic, LiveOps events, and backend boundaries for production games.

<p>
  <a href="https://github.com/HoNgocThaiGameDev?tab=repositories">
    <img src="https://img.shields.io/badge/GitHub-Repositories-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub repositories" />
  </a>
  <a href="#published-games">
    <img src="https://img.shields.io/badge/Published-Google_Play-34A853?style=for-the-badge&logo=googleplay&logoColor=white" alt="Published games" />
  </a>
  <a href="#selected-engineering-work">
    <img src="https://img.shields.io/badge/Focus-C%23_.NET_Unity-512BD4?style=for-the-badge&logo=dotnet&logoColor=white" alt="C# .NET Unity" />
  </a>
</p>

</div>

---

## What I Build

I build gameplay-adjacent backend and service logic for games: reward flows, progression systems, save-state handling, LiveOps event rules, API contracts, Firebase/Photon integrations, and tools that make game features easier to operate after release.

My current focus is writing game code that is easy to review: clear state transitions, defensive save migration, testable time logic, explicit edge-case handling, and behavior that QA can verify from a spec.

## Engineering Focus

| Area | Practical Ownership |
| --- | --- |
| LiveOps events | Event trigger rules, daily reset, cooldown, reward claim, popup state, tracking hooks |
| Player state | Save data shape, migration, versioning, rollback-safe progress, persistence boundaries |
| Game backend | Service/API logic, admin/support flows, clean contracts between client and backend |
| Platform integration | Firebase, Photon, Unity client communication, runtime debugging |
| Quality | NUnit tests, reviewable code, edge-case coverage, production-risk thinking |

## Published Games

| Product | Platform | Demo | Focus |
| --- | --- | --- | --- |
| [Conveyer Craze: Card Sort](https://play.google.com/store/apps/details?id=com.NebulaSoftStudio.ConveyerCrazeCardSortPuzzle) | Google Play | [Video demo](https://drive.google.com/file/d/13uM9Clp1OSWHNPoUWi7ML1pGx7ZwWjDM/view?usp=sharing) | 3D card-sorting puzzle game with mobile gameplay flow |
| [Hyper Gunner](https://play.google.com/store/apps/details?id=com.DefaultCompany.HyperGunner) | Google Play | [Video demo](https://drive.google.com/file/d/1WqkOJWwkruTGs9fmKhWGQRR6GihPHoU0/view?usp=sharing) | Strategy/action game with combat, upgrades, and progression |

## Selected Engineering Work

| Project | Stack | What It Shows |
| --- | --- | --- |
| [Comeback Bonus LiveOps Test](https://github.com/HoNgocThaiGameDev/comeback-bonus-liveops-test) | C#, .NET, NUnit | LiveOps event state machine, save migration, cooldown rules, reward flow, anti-cheat time boundaries, unit tests |
| [Piano Tile Core Game Demo](https://github.com/HoNgocThaiGameDev/Piano-Tile-Core-Game-Demo) | Unity, C# | Core gameplay loop, input timing, game-state organization |
| [Protect Street Demo](https://github.com/HoNgocThaiGameDev/Protect_Street_Demo) | Unity, C# | Gameplay systems, project structure, combat/progression logic |
| [Shooter Defense](https://github.com/HoNgocThaiGameDev/Shooter-Defense) | Unity, C# | Shooter-defense gameplay logic and C# system organization |

## Technical Stack

| Category | Tools |
| --- | --- |
| Languages | C#, C++, JavaScript/TypeScript |
| Backend | .NET, ASP.NET Core, REST APIs, PostgreSQL |
| Game tech | Unity, Photon, Firebase |
| Testing | NUnit, unit-testable service logic, edge-case test design |
| Workflow | Git, GitHub, readable PR-style documentation, debugging from logs and repro steps |

## How I Approach Game Systems

- Start from the PRD/spec and clarify ambiguous event rules before coding.
- Keep configuration data separate from controller logic so rewards, cooldowns, and balance values can be tuned safely.
- Treat save state as production data: version it, migrate it, and avoid overwriting player progress.
- Use injectable time providers for testability and prepare production paths for trusted/server time.
- Write focused tests around edge cases: first-time user, rollback time, fast-forward time, cooldown boundaries, reward failure, and old-save migration.
- Prefer explicit event hooks for UI, Missions, analytics, and other systems instead of hidden coupling.

## Current Direction

I am strengthening my game backend and LiveOps skill set around service architecture, player-state persistence, reward systems, production debugging, API boundaries, Firebase/Photon integration, and reliable C# test coverage.

---

<p align="center">
  Open to Game Backend, Unity LiveOps, and C#/.NET game-service opportunities.
</p>
