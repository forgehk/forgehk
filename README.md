<p align="center">
  <a href="https://hkforge.dev"><img src="assets/header.svg" width="100%" alt="Hasan Karakra. Software engineer: production platforms, AI and machine learning, security tooling, systems software."/></a>
</p>

**Hasan Karakra** · Software engineering · ML systems · Security · Distributed systems

I build and run production software, then dig into the systems underneath it. I'm a Senior Software Engineer at Farmacia Group, the founder of [Dusklayer](https://dusklayer.com) and [DarkForge AI](https://darkforgeai.com), and a computer science student at CSULB.

[Portfolio](https://hkforge.dev) · [LinkedIn](https://www.linkedin.com/in/hasan-karakra-ba94a440b/) · [All projects](PROJECTS.md)

## Featured engineering

| Repository | What makes it interesting | Proof |
|---|---|---|
| [forge-lm](https://github.com/forgehk/forge-lm) | A language model built end to end and trained from random weights: tokenizer, transformer and trainer in PyTorch, then inference written a second time in Rust with no dependencies. | 65 tests. The two implementations agree on every logit to within 1.2e-5. |
| [quorum](https://github.com/forgehk/quorum) | Raft consensus as a deterministic state machine, so a whole cluster, its network and its failures run from one seed. | A linearizability checker judges each run: 1,500 seeds, about 990,000 operations, no violation. |
| [anvil](https://github.com/forgehk/anvil) | A security gateway between an AI client and its MCP tool servers: allow and deny rules, human approval, secret redaction, tool pinning, a hash-chained audit log. | 206 tests on Linux and Windows. Its README lists what it does not defend against. |
| [Sentinel Vision](https://github.com/forgehk/sentinel-vision) | Camera analytics on detection and pose models exported to ONNX, running in the browser or as Windows apps. Counts people and never identifies them. | 41 rule tests and a [Windows release](https://github.com/forgehk/sentinel-vision/releases/latest) built in CI. |

Also pinned: [tiny-compiler](https://github.com/forgehk/tiny-compiler), a Pascal-style language compiled to MIPS assembly, and [darkforge-edr](https://github.com/forgehk/darkforge-edr), a Linux detection agent in Go. Newest: [forge-db](https://github.com/forgehk/forge-db), an LSM-tree storage engine tested on a simulated disk that loses power at any write.

## Production systems

- **Farmacia Group, six pharmacy locations in California.** I build and maintain the group site ([farmaciarx.com](https://farmaciarx.com)), the telehealth front door ([farmaciarxcare.com](https://farmaciarxcare.com)), the store sites for [Dinuba](https://farmaciadinuba.com) and [Anaheim](https://farmaciaanaheim.com), and the [supplement store](https://farmaciasupplements.com), in English and Spanish.
- **[Dusklayer](https://dusklayer.com).** Founder. A library of cinematic web pages sold as prompts, with live previews, accounts and plans.
- **Client storefronts.** [HairRx Lab](https://hairrxlab.com), telehealth, and [KeyKarams](https://keykarams.com), direct to consumer.

The stack behind each site is in [PROJECTS.md](PROJECTS.md).

## How I work

- Everything on this page has tests that pass in CI or a live site you can open.
- Engineering numbers come with the command that reproduces them.
- Every README says what the project does not do.

## More

[All projects](PROJECTS.md) · [Portfolio and case studies](https://hkforge.dev) · [DarkForge AI](https://darkforgeai.com) for client work ([info@darkforgeai.com](mailto:info@darkforgeai.com))

**Open to remote roles and project work only.** For roles, message me on [LinkedIn](https://www.linkedin.com/in/hasan-karakra-ba94a440b/).
