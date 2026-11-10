<div align="center">

```text
┌────────────────────────────────────────────────────────────────────────┐
│  rsanchez@operator:~                                                   │
├────────────────────────────────────────────────────────────────────────┤
│  Role       : Systems Operator · Autonomous Agent Engineer             │
│  OS         : Linux (Ubuntu 24.04 LTS / Arch Linux on libvirt)         │
│  Desktop    : GNOME 50 · Wayland-native                                │
│  Engine     : Hermes Agent · ED-209 Policy · R2-D2 Supervisor          │
│  Protocols  : Model Context Protocol (MCP) · AT-SPI · Chrome CDP       │
│  Stack      : Python · TypeScript · Rust · Go · Dart · Bash            │
└────────────────────────────────────────────────────────────────────────┘
```

[![Autonomous Tools](https://img.shields.io/badge/Autonomous%20Tools-9%20Published-blue?style=flat-square)](https://github.com/rudysanchez-mfb?tab=repositories)
[![License](https://img.shields.io/badge/License-Apache%202.0-orange?style=flat-square)](https://www.apache.org/licenses/LICENSE-2.0)
[![Platform](https://img.shields.io/badge/Platform-Linux%20%2F%20Wayland-success?style=flat-square&logo=linux&logoColor=white)](https://github.com/rudysanchez-mfb/gnome-wayland-computer-use)
[![Protocol](https://img.shields.io/badge/Protocol-MCP%20stdio-6E56CF?style=flat-square)](https://github.com/rudysanchez-mfb/council-mcp)
[![Profile Views](https://komarev.com/ghpvc/?username=rudysanchez-mfb&color=blue&style=flat-square&label=Profile%20Views)](https://github.com/rudysanchez-mfb)

</div>

I build the unglamorous layer that makes autonomous coding agents survivable in production: deterministic policy enforcement, capability supervision, and verification tooling that refuses to lie about what it proved.

Most tooling treats LLMs as infallible products. I treat them as high-variance workers with a schedule, where the real engineering is everything wrapped around them — rule provenance you can audit, capability death you can detect, demo videos you can mechanically verify, and consoles that stop needing humans to click through them at 2 AM.

---

## 🛠️ Systems & Tooling

### 🛡️ Agent Policy & Deliberation
- **[operator-guards](https://github.com/rudysanchez-mfb/operator-guards)** — Coordinated Python library and Hermes plugins for **ED-209** deterministic behavioral rules and **R2-D2** capability observation, incident ledgers, and kill-authorized recovery. *(659 tests, stdlib runtime)*
- **[council-mcp](https://github.com/rudysanchez-mfb/council-mcp)** — Multi-model deliberation over stdio MCP. Fans out to 4 frontier models in parallel with bounded judge synthesis, latency budgets, and `classify_degraded` thinking-tag/CoT stripping. *(34 tests)*

### 🖥️ Native Desktop & Store Automation
- **[gnome-wayland-computer-use](https://github.com/rudysanchez-mfb/gnome-wayland-computer-use)** — Native GNOME Wayland desktop control for AI agents with a companion GNOME Shell extension, AT-SPI tree targeting, and an agent UX contract.
- **[store-console](https://github.com/rudysanchez-mfb/store-console)** — Google Play Console and Apple App Store Connect automation via Playwright over Chrome DevTools Protocol (CDP) on an active profile.

### 🎬 Verification & PR Cinema
- **[pr-cinema](https://github.com/rudysanchez-mfb/pr-cinema)** — Assertion-gated PR showreel pipeline: records Playwright takes, burns captions, renders dynamic bookends, and mechanically verifies cuts (`verify-cut.mjs`) before release.
- **[music-video-demo](https://github.com/rudysanchez-mfb/music-video-demo)** — Scores and cuts software takes to music video pacing with beat-synced cards and burned captions; includes `add-demo-track`.
- **[read-media](https://github.com/rudysanchez-mfb/read-media)** — Multimodal bridge for text-only coding agents: ffmpeg scene-change keyframes + local whisper.cpp speech transcription + vision synthesis.

### ⚡ Operations & Observability
- **[hermes-skills](https://github.com/rudysanchez-mfb/hermes-skills)** — Curated 10-skill Hermes skills tap: `scope-fence`, `plan-gate`, `adversarial-verify`, `ruthless-editor`, `memory-hygiene`, `storage-space-check` (8 unit tests), and core change safety.
- **[hermes-dashboard](https://github.com/rudysanchez-mfb/hermes-dashboard)** — Web Command Center for monitoring Hermes agent sessions, background daemons, and system status (Express 5 backend + vanilla JS components).

---

## 💻 Tech Stack & Runtime

<div align="center">

**Languages**  
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![Dart](https://img.shields.io/badge/Dart-0175C2?style=flat-square&logo=dart&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)

**Platform, Infrastructure & Protocols**  
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![GNOME Wayland](https://img.shields.io/badge/GNOME-Wayland-4A86CF?style=flat-square&logo=gnome&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-Containers-2496ED?style=flat-square&logo=docker&logoColor=white)
![systemd](https://img.shields.io/badge/systemd-Daemons-000000?style=flat-square&logo=systemd&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-Protocol-6E56CF?style=flat-square)
![Playwright](https://img.shields.io/badge/Playwright-Automation-2EAD33?style=flat-square&logo=playwright&logoColor=white)

</div>

---

<details>
<summary><b>Operating Principles</b></summary>

<br>

- **Prove it or drop it.** A green check that verifies nothing is worse than a red one that tells the truth. Every check must assert real state.
- **Verification before publication.** Secrets scanned, personal paths stripped, licenses chosen, and tests actually executed — never claimed from intent.
- **Same-user guards are not an OS boundary.** I state that plainly in documentation rather than pretend an application-level hook is a kernel sandbox.
- **Boring beats clever.** A bounded retry loop with a hard deadline outlives an elegant unbounded architecture every day of the week.

</details>

---

<div align="center">

<img src="https://streak-stats.demolab.com/?user=rudysanchez-mfb&theme=dark&hide_border=true" alt="GitHub Streak" />

</div>
