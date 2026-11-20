<p align="center">
  <a href="https://hkforge.dev"><img src="assets/header.svg" width="100%" alt="Hasan Karakra. Software engineer: production platforms, AI and machine learning, security tooling, systems software."/></a>
</p>

**Software engineering · AI and machine learning · Security · Distributed systems**

I'm a Senior Software Engineer at Farmacia Group, where I build and run the pharmacy group's sites, telehealth intake and stores. I'm also the founder of [Dusklayer](https://dusklayer.com) and [DarkForge AI](https://darkforgeai.com), and I study computer science at CSULB.

On my own time I build the layers underneath that kind of software: a language model trained from random weights with its own inference engine, consensus and storage engines tested against simulated failures, detection pipelines, and security tooling.

[Portfolio](https://hkforge.dev) · [LinkedIn](https://www.linkedin.com/in/hasan-karakra-ba94a440b/) · [All projects](PROJECTS.md) · [DarkForge AI](https://darkforgeai.com) for client work

## Selected engineering

| Project | What it is | Proof you can check |
|---|---|---|
| [forge-lm](https://github.com/forgehk/forge-lm) | A language model built end to end and trained from random weights: byte-level BPE tokenizer, Llama-style transformer in PyTorch, and an inference engine in Rust with no dependencies. | 65 tests. The Rust engine reproduces PyTorch's logits to 1e-5 at every position. |
| [quorum](https://github.com/forgehk/quorum) | Raft consensus in Go as a deterministic state machine, with a seeded simulator for partitions, crashes and message loss. | A linearizability checker judges every run: 1,500 seeds, about 990,000 operations, no violation. |
| [anvil](https://github.com/forgehk/anvil) | Security gateway that sits between an AI client and its MCP tool servers: allow and deny rules, human approval, secret redaction, tool pinning, audit log. | 206 tests on Linux and Windows. The README says what it does not defend against. |
| [Sentinel Vision](https://github.com/forgehk/sentinel-vision) | Camera analytics on YOLO detection and pose models exported to ONNX, running in the browser or as Windows apps. Counts people and never identifies them. | Rule engine tests and a [Windows release](https://github.com/forgehk/sentinel-vision/releases/latest) built in CI. |
| [tiny-compiler](https://github.com/forgehk/tiny-compiler) | A Pascal-style language compiled to MIPS-32 assembly: lexer, parser, AST, code generator and a reference interpreter. | 41 tests. The output runs on [mips-emulator](https://github.com/forgehk/mips-emulator). |
| [darkforge-edr](https://github.com/forgehk/darkforge-edr) | Linux endpoint detection agent in Go: process telemetry from /proc through a YAML rule engine to JSON alerts. | 47 tests under the race detector. Linux only, and the README says where it stops. |

Newest: [forge-db](https://github.com/forgehk/forge-db), an LSM-tree storage engine in Rust tested on a simulated disk that cuts the power at any storage operation. The rest, about twenty repositories with their test counts, is in [PROJECTS.md](PROJECTS.md).

## Production work

Farmacia Group runs six pharmacies in California. I built and maintain its group site ([farmaciarx.com](https://farmaciarx.com)), its telehealth front door ([farmaciarxcare.com](https://farmaciarxcare.com)), the store sites for [Dinuba](https://farmaciadinuba.com) and [Anaheim](https://farmaciaanaheim.com), and its [supplement store](https://farmaciasupplements.com), in English and Spanish. Outside the group I have shipped telehealth and direct-to-consumer storefronts ([HairRx Lab](https://hairrxlab.com), [KeyKarams](https://keykarams.com)) and my own product, [Dusklayer](https://dusklayer.com).

Case studies are on [hkforge.dev](https://hkforge.dev), and the stack behind each site is in [PROJECTS.md](PROJECTS.md).

## How I work

- A repository goes public when its tests pass in CI, and each one links the workflow so you can see the last run.
- Numbers come with the command that reproduces them: seeds, benchmarks, parity checks.
- Every README says what the project does not do and what was not tested.

**Open to remote roles and project work only.** For roles, message me on [LinkedIn](https://www.linkedin.com/in/hasan-karakra-ba94a440b/) or through [hkforge.dev](https://hkforge.dev). For client work, [info@darkforgeai.com](mailto:info@darkforgeai.com).
