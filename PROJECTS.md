# All projects

The full list behind [my profile](README.md). Everything here is in production, has a live site you can open, or ships with a test suite and a CI workflow you can inspect. Team projects, course projects and work in progress are labelled.

## In production

Farmacia Group runs six pharmacies in California. I build and run its sites, its telehealth front door and its stores.

| Site | What it does | Built with |
|---|---|---|
| [FarmaciaRx](https://farmaciarx.com) | Group site for six California pharmacies: store directory, prescription transfer and refill request forms, a compounding explainer, and a full Spanish mirror with hreflang. | HTML, CSS, JS, Netlify Forms |
| [FarmaciaRx Care](https://farmaciarxcare.com) | Telehealth front door for the same group: intake, review by a California licensed prescriber, then shipping or pharmacy pickup. There is no cart and no way to order past a prescriber. English and Spanish. | HTML, CSS, JS, Netlify |
| [Farmacia Dinuba](https://farmaciadinuba.com) | Bilingual site for the group's Central Valley store: real store photography, a video tour, a prescription bottle you can drag to turn, and a three step transfer flow. Takes no health details through the site, by design. | HTML, CSS, JS, Canvas |
| [Farmacia Anaheim](https://farmaciaanaheim.com) | Site for the group's Anaheim pharmacy, built as a custom WordPress theme: services, compounding and immunization pages, prescription refill, new patient and contact forms that land in the pharmacist's inbox. | WordPress, PHP |
| [Farmacia Wellness](https://farmaciasupplements.com) | Bilingual supplement store for the group: cart and checkout, bundles, wholesale and in store pickup. | HTML, CSS, JS, Netlify, Authorize.Net |
| [HairRx Lab](https://hairrxlab.com) | Telehealth storefront for a compounded prescription, with a scroll pinned sequence and a before and after slider. | Next.js 14, Framer Motion, Lenis |
| [KeyKarams](https://keykarams.com) | D2C product page with a three.js product viewer and a custom cart that hands off to Shopify checkout. | three.js, Shopify, Klaviyo |

**In development:** [Kormiia](https://kormiia.com), a telehealth site for a compounded prescription. California only.

## Products

| Product | What it is | Built with |
|---|---|---|
| [Dusklayer](https://dusklayer.com) | Founder. A library of cinematic web pages sold as prompts. Pick a scene, section or product film, choose a look, and paste its prompt into Claude Code, Cursor or v0 to rebuild it in your own stack. 22 layers with nine looks each, live previews, accounts and three plans. | TypeScript, Netlify |
| [Nyko](https://nyko.app) | Private AI assistant PWA: chat, vision and PDFs, voice, custom bots, memory, live canvas. | Vanilla JS modules, service worker |
| [CyberForge](https://cyberforge-cecs491a.netlify.app) | Adaptive web security training platform: a 32 question placement, a prerequisite skill graph through 16 lessons and a capstone, labs graded on the server, a nine tool security toolkit. CSULB senior project, team of five, in progress. | Python engine, vanilla JS, Netlify Functions running Pyodide, Supabase, Three.js |

## AI and machine learning

| Project | What it is | Built with |
|---|---|---|
| [forge-lm](https://github.com/forgehk/forge-lm) | A language model built end to end and trained from random weights: a byte-level BPE tokenizer, a Llama-style transformer (RMSNorm, rotary embeddings, SwiGLU) and its trainer, a single-file model format, and an inference engine in Rust with zero dependencies. The engine reproduces PyTorch's logits to 1e-5 at every position. | Python, PyTorch, Rust. 65 tests, CI on Linux and Windows |
| [Sentinel Vision](https://github.com/forgehk/sentinel-vision) | Camera analytics that turns footage into timestamped statuses: desk presence, zone dwell and occupancy, front door alerts, head turn flags in an exam hall. YOLO26 detection and pose models exported to ONNX, running in the browser on WebAssembly or as four Windows apps. Counts people and never identifies them. [Windows release](https://github.com/forgehk/sentinel-vision/releases/latest). | Python, ONNX Runtime, JavaScript, three.js. 41 rule tests, release CI |

## Security

| Repo | What it is | Status |
|---|---|---|
| [anvil](https://github.com/forgehk/anvil) | Security gateway for MCP. Sits between an AI client and a tool server and enforces allow and deny rules, human approval, secret redaction, prompt injection scanning, tool pinning and a hash chained audit log. Stdlib only. | 206 tests, CI on Linux and Windows |
| [darkforge-edr](https://github.com/forgehk/darkforge-edr) | Linux endpoint detection agent in Go: /proc telemetry through a YAML rule engine, JSON lines alerts with MITRE tags. Evicts exited PIDs so PID reuse is re evaluated. | 47 tests, race detector CI |
| [honeytoken-sentinel](https://github.com/forgehk/honeytoken-sentinel) | Mint decoy AWS, GitHub and Stripe credentials and canary URLs; get alerted the moment one is touched. Unknown token ids answer exactly like real ones, so tokens cannot be enumerated. Stdlib only. | 19 tests |
| [pipeline-armor](https://github.com/forgehk/pipeline-armor) | CI security gate for GitHub Actions: regex secret scanner with an entropy floor, AST pattern scanner, YAML policy engine. Its own CI fails if the gate ever stops blocking the bundled vulnerable demo. | 19 tests |
| [secret-rotator](https://github.com/forgehk/secret-rotator) | Rotate API keys across providers in six steps: snapshot, provision, update the store, verify, grace period, revoke. Any failure rolls back from the snapshot, and every step lands in a tamper evident audit log. | 14 tests |
| [dns-doctor](https://github.com/forgehk/dns-doctor) | One command audit of a domain's DNS, CAA, TLS, SPF, DKIM, DMARC, MTA-STS and HTTP security headers, with a letter grade per check and a punch list. | 36 tests |
| [nextjs-auth-armor](https://github.com/forgehk/nextjs-auth-armor) | Hardened Next.js 14 starter: Supabase magic link auth, Row Level Security migrations, CSP middleware, honeypot forms. | Typecheck, lint and build CI |
| [phish-forge](https://github.com/forgehk/phish-forge) | Score an .eml for phishing from header, URL and body heuristics, with hand rolled typosquat and homoglyph checks. CLI and FastAPI service. | 30 tests |
| [ctf-toolkit](https://github.com/forgehk/ctf-toolkit) | Stdlib only CTF CLI: encoders, classical ciphers, hash identification and cracking, and small e, common modulus and Wiener RSA attacks written from first principles. | 36 tests |
| [steg-toolkit](https://github.com/forgehk/steg-toolkit) | Image steganography: LSB hide and extract, strings recovery, per channel entropy and LSB plane heatmaps. | 12 tests |
| [darkforge-cli](https://github.com/forgehk/darkforge-cli) | One CLI over the tools above: scan a domain, audit a repo or score an email, with severity grading and JSON reports. | 15 tests |

## Systems and compilers

| Repo | What it is | Status |
|---|---|---|
| [quorum](https://github.com/forgehk/quorum) | Raft consensus in Go, written as a deterministic state machine: Pre-Vote, CheckQuorum, log compaction, snapshot transfer, exactly-once commands. A seeded simulator injects partitions, crashes and message loss, and a linearizability checker judges what the clients saw. 1,500 seeds and 990,000 operations without a violation. No dependencies. | 34 tests, race detector CI |
| [forge-db](https://github.com/forgehk/forge-db) | Embedded LSM-tree key-value store in Rust: write-ahead log, sorted tables with Bloom filters, leveled compaction, and a manifest replaced atomically. All storage goes through one trait, and a simulated disk cuts the power at any storage operation, including during recovery. A checker then demands that what comes back is an allowed prefix of the acknowledged writes. No dependencies. | 67 tests, CI on Linux and Windows |
| [tiny-compiler](https://github.com/forgehk/tiny-compiler) | A Pascal style language that compiles to MIPS 32 assembly (SPIM or MARS): lexer, recursive descent parser, AST, codegen and a reference interpreter in about 700 lines of Python. | 41 tests |
| [mips-emulator](https://github.com/forgehk/mips-emulator) | MIPS 32 assembler and single cycle emulator in C++17 with trace and memory dump modes. Runs textbook programs end to end. | 15 tests, CI runs three example programs |
| [cecs327-smart-parking](https://github.com/forgehk/cecs327-smart-parking) | Hand built TCP framing, idempotent request reply, a pub sub broker, registry based group messaging and log replay recovery, from the Python standard library. Team project, CECS 327. | [Live demo](https://cecs327-smart-parking.netlify.app), 35 tests |
| [bigint-cpp](https://github.com/forgehk/bigint-cpp) | Arbitrary precision integers in C++17 with operator overloading, tail recursive factorial and Fibonacci, and a Collatz walker. | 78 checks |

## Tooling

| Repo | What it is | Status |
|---|---|---|
| [lead-foundry](https://github.com/forgehk/lead-foundry) | Normalize, dedupe and ICP score lead CSVs locally, with a pluggable enrichment hook and YAML rules. | 30 tests |
| [pixel-forge](https://github.com/forgehk/pixel-forge) | One product photo to HSV recolored catalog variants with Pillow. Deterministic and offline. | 17 tests |

## Stack

```text
Languages   Python · Go · Rust · C++ · TypeScript · JavaScript · SQL · Bash
Backend     FastAPI · Node · Netlify Functions · Supabase · SQLite · Pyodide
Frontend    Next.js · React · vanilla JS · Three.js · Canvas · WebGL · WordPress
Commerce    Shopify · Authorize.Net · Klaviyo · bilingual EN/ES storefronts
ML          PyTorch · transformers and BPE tokenizers from scratch · YOLO · ONNX Runtime ·
            WebAssembly · OpenCV
Systems     Raft · LSM-tree storage · deterministic simulation · linearizability and
            crash-consistency checking · compilers · emulators
Security    MCP and prompt injection defense · YAML rule engines · canary tokens · SAST
            and secret scanning · CSP and security headers · DNS, SPF, DMARC and CAA
Tooling     pytest · Go test · cargo test · Playwright · GitHub Actions · Docker · Netlify
```
