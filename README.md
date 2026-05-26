<h1 align="center">@forgehk</h1>

<p align="center">
  <em>Engineer · Security · Systems · Building <a href="https://darkforgeai.com">DarkForge AI</a></em>
</p>

<p align="center">
  <a href="https://forgehk.github.io"><img alt="Site" src="https://img.shields.io/badge/site-forgehk.github.io-0EA5E9?style=for-the-badge"/></a>
  <a href="mailto:info@darkforgeai.com"><img alt="Email" src="https://img.shields.io/badge/contact-info%40darkforgeai.com-EF4444?style=for-the-badge"/></a>
</p>

---

I build **security tooling**, **systems software**, and **AI-accelerated full-stack apps**. Every repo below is mine, public, has working code, and ships with tests. No tutorials, no forks.

### Pinned work

#### Security & DevSecOps

- **[honeytoken-sentinel](https://github.com/forgehk/honeytoken-sentinel)** — Self-hosted Thinkst-Canary-style tripwire. Mints decoy AWS/GitHub/Stripe credentials and canary URLs; alerts the second one is touched. Stdlib-only HTTP listener, atomic JSON registry, Slack webhook. *19/19 tests.* `python`
- **[darkforge-edr](https://github.com/forgehk/darkforge-edr)** — Lightweight endpoint detection agent. YAML rule engine over process, file, and network telemetry, with a SQLite alert store and a Next.js console (see below). `go` `sqlite`
- **[pipeline-armor](https://github.com/forgehk/pipeline-armor)** — Drop-in DevSecOps gate for GitHub Actions: SAST + SCA + secrets scanner + container scan. Ships with a deliberately vulnerable demo app the gate catches. *12/12 tests.* `python` `actions` `semgrep` `trivy`
- **[darkforge-edr-dashboard](https://github.com/forgehk/darkforge-edr-dashboard)** — Next.js 14 + Tailwind console that consumes the EDR feed. Filterable alert grid, severity timeline, host drill-down. `nextjs` `tailwind`

#### Systems & Compilers

- **[tiny-compiler](https://github.com/forgehk/tiny-compiler)** — A Pascal-style language that actually compiles to **MIPS-32 assembly**. Full lexer → parser → AST → codegen pipeline in ~700 lines. *25/25 tests.* Pairs with `mips-emulator`. `python` `compiler`
- **[mips-emulator](https://github.com/forgehk/mips-emulator)** — MIPS-32 instruction-set emulator in C++17. Decodes R/I/J-type, executes a useful subset of arithmetic / branch / memory / syscall ops. *16/16 tests.* `cpp` `systems`

### The rest

| Area | Repos |
|---|---|
| **Offensive / red team** | [ctf-toolkit](https://github.com/forgehk/ctf-toolkit) · [steg-toolkit](https://github.com/forgehk/steg-toolkit) · [phish-forge](https://github.com/forgehk/phish-forge) |
| **Defensive AppSec** | [secret-rotator](https://github.com/forgehk/secret-rotator) · [dns-doctor](https://github.com/forgehk/dns-doctor) · [nextjs-auth-armor](https://github.com/forgehk/nextjs-auth-armor) |
| **Meta / orchestration** | [darkforge-cli](https://github.com/forgehk/darkforge-cli) — runs the whole security suite through one grade-A-to-F CLI |
| **CS depth** | [bigint-cpp](https://github.com/forgehk/bigint-cpp) · [polyglot-sort-grand-prix](https://github.com/forgehk/polyglot-sort-grand-prix) · [prolog-ufo-puzzle](https://github.com/forgehk/prolog-ufo-puzzle) |
| **Frontend / viz** | [algoviz](https://github.com/forgehk/algoviz) (Three.js 3D sort visualizer) · [pixel-forge](https://github.com/forgehk/pixel-forge) · [lead-foundry](https://github.com/forgehk/lead-foundry) |

### How I work

```text
Languages   Python · Go · C++ · TypeScript · SQL · Bash · Prolog · MIPS asm
Backend     FastAPI · Node · Supabase · SQLite · REST · subprocess orchestration
Frontend    Next.js · React · Tailwind · Three.js
Security    SAST (Semgrep) · SCA (Trivy) · secrets (gitleaks) · DNS/SPF/DKIM/DMARC ·
            TLS · YAML rule engines · canary tokens · STRIDE threat modeling
Tooling     pytest · Go test · CMake · GitHub Actions · Docker
```

### Currently shipping in public

Compilers, distributed systems, and a small language model of my own. Repos drop here when they're test-passing — not before.

---

<p align="center">
  📬 <a href="mailto:info@darkforgeai.com">info@darkforgeai.com</a> · 🌐 <a href="https://forgehk.github.io">forgehk.github.io</a>
</p>
