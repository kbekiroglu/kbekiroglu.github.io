---
title: "AI-Assisted Engineering: Adoption and Internal Tooling"
excerpt: "Claude Code and Codex across the controls team, Control Flow diagrams generated from source with Mermaid, and an internal telemetry diagnostic tool for non-engineers.<br/><img src='/images/ai-portfolio.png' width='550' height='600'>"
collection: portfolio
---

Three things I lead at SharkNinja: getting the controls team using LLM tools in daily work, generating our control architecture diagrams from source instead of drawing them, and an internal tool that lets non-engineers debug products from telemetry.

<img src='/images/ai-portfolio.png' width='700'>

Where it landed
======

* The same headcount supports about 40% more concurrent projects
* Control Flow diagrams come out of the source, so they no longer go stale between firmware revisions
* Product managers, QA and support triage issues from unit CSV data without pulling in a controls engineer
* Design decisions get written down with the reasoning, because writing them down is now cheap

Team adoption
======

I standardized how the team uses Claude Code and OpenAI Codex. I did it through a few power users and shared prompt patterns rather than a mandate, because a mandate gets you compliance and no learning.

Where it actually gets used:

* Controller scaffolding, sensor driver boilerplate, test harness code, embedded utilities
* Algorithm exploration and tradeoff analysis early in a project
* Plotting and statistics on experimental sensor data
* Diff summaries, PR review help, release notes
* Confluence through an MCP integration, so design docs and specs get written and cross-linked where the team already looks for them

Control Flow diagrams in Mermaid
======

Control Flow is the control architecture specification standard I created here, and it is now required on every controls project in the company. It captures the state machine, mode transitions, interrupt priorities, and the safety and fault paths before anybody writes firmware.

The standard worked. Keeping it current did not. The diagrams were drawn by hand, so they cost real time to produce and went stale the first time the firmware changed. Once a diagram is stale, engineers stop opening it and go read the code instead, and then design reviews turn into arguments about whether the picture is accurate.

So we moved Control Flow to Mermaid and generate the state machine and sequence diagrams from the control specification and the firmware.

Mermaid diagrams are plain text, so they sit in the repo next to the code and get reviewed in a pull request like any other change. They render in Confluence, GitHub and Markdown from one source, with no drawing tool in the loop. And they are cheap enough to regenerate that nobody has to protect them.

What changed:

* Architecture docs get updated during development instead of at the end of a program
* New engineers and our offshore firmware partners can learn a product's control structure from a diagram that matches how it actually behaves
* Design reviews argue about the state machine
* Interrupt priorities, mode transitions and safety paths stay explicit on every project, which is the whole point of the standard

Internal product diagnostics
======

I led an internal tool that gives product managers, QA and customer support engineers a way to answer product-specific questions without going through controls.

They can ask in plain language how a feature works or why a unit is behaving a certain way. They can upload a unit's CSV telemetry and get a first pass on sensor anomalies, thermal and fluid behavior deviations, control loop faults, and edge case triggers. It runs against our own product documentation and known failure modes, so the answers are about our products and not generic.

Support and QA now handle the first layer themselves, controls engineers stop repeating the same first-line diagnosis, and a field or QA issue gets triaged in hours.
