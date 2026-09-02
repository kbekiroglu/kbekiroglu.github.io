---
title: "AI-Assisted Engineering: Adoption and Internal Tooling"
excerpt: "LLM-assisted workflows standardized across the controls team, Control Flow architecture diagrams generated instead of hand-drawn, and an internal telemetry diagnostic tool for non-engineers.<br/><img src='/images/ai-portfolio.png' width='550' height='600'>"
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

Control Flow diagrams in Mermaid and draw.io
======

Control Flow is the control architecture specification standard I created here. It is required on every controls project in the company, and it captures the state machine, mode transitions, interrupt priorities and the safety and fault paths before anybody writes firmware.

The standard worked. Upkeep did not. Diagrams were drawn by hand, so they went stale the first time firmware changed, and a stale diagram is one nobody opens.

We moved them to Mermaid and draw.io, generated from the control specification and the firmware. Both are text files, so they live in the repo next to the code and render straight into Confluence and GitHub. They are cheap enough to regenerate that nobody has to protect them, so architecture docs now stay current during development, and a new engineer or an offshore firmware partner can learn a product from a diagram that matches how it behaves.

Internal product diagnostics
======

I led an internal tool that gives product managers, QA and customer support engineers a way to answer product-specific questions without going through controls.

They can ask in plain language how a feature works or why a unit is behaving a certain way. They can upload a unit's CSV telemetry and get a first pass on sensor anomalies, thermal and fluid behavior deviations, control loop faults, and edge case triggers. It runs against our own product documentation and known failure modes, so the answers are about our products and not generic.

Support and QA now handle the first layer themselves, controls engineers stop repeating the same first-line diagnosis, and a field or QA issue gets triaged in hours.
