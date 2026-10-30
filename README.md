<h1 align="center">Hasan Karakra</h1>

<p align="center">
  <em>Computer science at CSULB · founder of <a href="https://darkforgeai.com">DarkForge AI</a> · security tooling, systems software and production web platforms</em>
</p>

<p align="center">
  <a href="https://hkforge.dev"><img alt="Portfolio" src="https://img.shields.io/badge/portfolio-hkforge.dev-0EA5E9?style=for-the-badge"/></a>
  <a href="mailto:info@darkforgeai.com"><img alt="Email" src="https://img.shields.io/badge/contact-info%40darkforgeai.com-EF4444?style=for-the-badge"/></a>
</p>

---

Twelve live platforms, a senior project in web security, and the repositories below. Everything listed here has working code, a test suite or continuous integration, or a live demo you can open. Case studies with screenshots are on [hkforge.dev](https://hkforge.dev).

### Live

| Project | What it is | Built with |
|---|---|---|
| [CyberForge](https://cyberforge-cecs491a.netlify.app) | Adaptive web security training platform: a 32 question placement, a prerequisite skill graph through 16 lessons and a capstone, labs graded on the server, a nine tool security toolkit. CSULB senior project, team of five, in progress. | Python engine, vanilla JS, Netlify Functions running Pyodide, Supabase, Three.js |
| [Farmacia Wellness](https://farmaciasupplements.com) | Bilingual supplement store for a pharmacy group: 14 products, cart and checkout, wholesale and pickup, policies. | HTML, CSS, JS, Netlify, Authorize.Net |
| [HairRx Lab](https://hairrxlab.com) | Telehealth storefront for a compounded prescription, with a scroll pinned sequence and a before and after slider. | Next.js 14, Framer Motion, Lenis |
| [KeyKarams](https://keykarams.com) | D2C landing page with a three.js product viewer and a custom cart that hands off to Shopify checkout. | three.js, Shopify, Klaviyo |
| [FarmaciaRx](https://farmaciarx.com) and [FarmaciaRx Care](https://farmaciarxcare.com) | Six location landing page and telehealth front door on one design system, English and Spanish with hreflang. | HTML, CSS, JS, Netlify forms |
| [Nyko](https://nyko.app) | Private AI assistant PWA: chat, vision and PDFs, voice, custom bots, memory, live canvas. | Vanilla JS modules, service worker |
| [Hyperswarm](https://inquisitive-semifreddo-b68115.netlify.app) | Twin stick roguelite written from scratch in one 182 KB HTML file, with a WebGL bloom pass. | Canvas 2D, WebGL |
| [Universe Drift](https://amazing-flan-f43887.netlify.app) | Real time solar system with free flight, a narrated tour and per planet data. | three.js |
| [Fluid Cursor](https://fluid-cursor-demo.netlify.app) | 4 KB zero dependency spring physics cursor with a data attribute API and a live playground. | JavaScript |
| [Distributed Smart Parking](https://cecs327-smart-parking.netlify.app) | Fault tolerant distributed system in stdlib Python, running in the browser as Web Workers with fault injection. CECS 327. | Python, Web Workers |

Also live: [darkforgeai.com](https://darkforgeai.com) and [kormiia.com](https://kormiia.com).

### Security

| Repo | What it is | Status |
|---|---|---|
| [darkforge-edr](https://github.com/forgehk/darkforge-edr) | Linux endpoint detection agent in Go: /proc telemetry through a YAML rule engine, JSON lines alerts with MITRE tags. Evicts exited PIDs so PID reuse is re evaluated. | 37 tests, race detector CI |
| [honeytoken-sentinel](https://github.com/forgehk/honeytoken-sentinel) | Mint decoy AWS, GitHub and Stripe credentials and canary URLs; get alerted the moment one is touched. Unknown token ids answer exactly like real ones, so tokens cannot be enumerated. Stdlib only. | 19 tests |
| [pipeline-armor](https://github.com/forgehk/pipeline-armor) | CI security gate for GitHub Actions: regex secret scanner with an entropy floor, AST pattern scanner, YAML policy engine. Its own CI fails if the gate ever stops blocking the bundled vulnerable demo. | 19 tests |
| [nextjs-auth-armor](https://github.com/forgehk/nextjs-auth-armor) | Hardened Next.js 14 starter: Supabase magic link auth, Row Level Security migrations, CSP middleware, honeypot forms. | Typecheck, lint and build CI |
| [ctf-toolkit](https://github.com/forgehk/ctf-toolkit) | Stdlib only CTF CLI: encoders, classical ciphers, hash identification and cracking, and small e, common modulus and Wiener RSA attacks written from first principles. | 36 tests |
| [phish-forge](https://github.com/forgehk/phish-forge) | Score an .eml for phishing from header, URL and body heuristics, with hand rolled typosquat and homoglyph checks. CLI and FastAPI service. | 23 tests |
| [steg-toolkit](https://github.com/forgehk/steg-toolkit) | Image steganography: LSB hide and extract, strings recovery, per channel entropy and LSB plane heatmaps. | Small, tested roundtrip |

### Systems and compilers

| Repo | What it is | Status |
|---|---|---|
| [tiny-compiler](https://github.com/forgehk/tiny-compiler) | A Pascal style language that compiles to MIPS 32 assembly (SPIM or MARS): lexer, recursive descent parser, AST, codegen and a reference interpreter in about 700 lines of Python. | 41 tests |
| [mips-emulator](https://github.com/forgehk/mips-emulator) | MIPS 32 assembler and single cycle emulator in C++17 with trace and memory dump modes. Runs textbook programs end to end. | 15 tests, CI runs three example programs |
| [bigint-cpp](https://github.com/forgehk/bigint-cpp) | Arbitrary precision integers in C++17 with operator overloading, tail recursive factorial and Fibonacci, and a Collatz walker. | 78 checks |
| [cecs327-smart-parking](https://github.com/forgehk/cecs327-smart-parking) | Hand built TCP framing, idempotent request reply, a pub sub broker, registry based group messaging and log replay recovery, from the Python standard library. | Live demo, 7 failure scenarios |

### Tooling

| Repo | What it is | Status |
|---|---|---|
| [lead-foundry](https://github.com/forgehk/lead-foundry) | Normalize, dedupe and ICP score lead CSVs locally, with a pluggable enrichment hook and YAML rules. | 19 tests |
| [pixel-forge](https://github.com/forgehk/pixel-forge) | One product photo to HSV recolored catalog variants with Pillow. Deterministic and offline. | 17 tests |
| [algoviz](https://github.com/forgehk/algoviz) | 3D sorting algorithm visualizer in vanilla Three.js with synced pseudocode. | Browser demo |

### How I work

```text
Languages   Python · Go · C++ · TypeScript · JavaScript · SQL · Bash
Backend     FastAPI · Node · Netlify Functions · Supabase · SQLite · Pyodide
Frontend    Next.js · React · vanilla JS · Three.js · Canvas · WebGL
Security    YAML rule engines · canary tokens · SAST and secret scanning · CSP and
            security headers · DNS, SPF, DMARC and CAA · threat modeling
Tooling     pytest · Go test · Playwright · GitHub Actions · Docker · Netlify
```

Repositories land here when they pass their tests, not before.

---

<p align="center">
  <a href="https://hkforge.dev">hkforge.dev</a> · <a href="mailto:info@darkforgeai.com">info@darkforgeai.com</a>
</p>
