---
title: "AI-Assisted Engineering — Adoption and Internal AI Tooling"
excerpt: "Drove Claude Code and OpenAI Codex adoption across the SharkNinja Control Systems team. Same headcount now supports approximately 40% more concurrent projects. Automated Control Flow state-machine diagram generation using Mermaid, so control architecture documentation stays in version control alongside the firmware. Also led an internal AI diagnostic tool that lets non-engineers ask product questions and analyze CSV telemetry to identify software or hardware issues.<br/><img src='/images/ai-portfolio.png' width='550' height='600'>"
collection: portfolio
---

As Senior Director of Control Systems Engineering, I lead the AI initiatives inside SharkNinja controls: standardizing LLM-assisted workflows across the engineering team, automating generation of our Control Flow architecture documentation, and building an internal AI diagnostic tool that lets non-engineers reason about product behavior directly from unit telemetry.

<img src='/images/ai-portfolio.png' width='700'>

Impact
======

* Same engineering headcount supports approximately **40% more concurrent projects**
* **Control Flow diagrams generated from source instead of drawn by hand**, so control architecture documentation no longer goes stale between firmware revisions
* Non-engineers now triage software and hardware issues from unit CSV data without controls-engineering time
* Shorter idea-to-prototype cycle time on new controls features
* Higher documentation coverage and design-decision traceability through MCP-integrated Confluence workflows

AI-assisted engineering — team adoption
======

Standardized how the Control Systems team uses **Claude Code** and **OpenAI Codex** in daily work. Rolled out through power-user pilots and shared prompt patterns rather than top-down mandate.

**Engineering workflows**

* **Code generation** — controller scaffolding, sensor-driver boilerplate, test-harness code, and embedded-system utilities
* **R&D and ideation** — algorithm exploration, alternative approaches to controls problems, tradeoff analysis
* **Data-analysis pipelines** — plotting, statistical analysis, and exploration of experimental sensor data
* **Code comparison and change-log automation** — diff summarization, PR review assistance, and release-note generation

**Documentation and knowledge capture**

* **Confluence via MCP integration** — design documents, meeting notes, and technical specs written, updated, and cross-linked directly in Confluence
* Documentation kept current at a granularity the team could not sustain manually
* Design decisions captured with the reasoning behind them, not only the final outcome

Automated Control Flow generation with Mermaid
======

Control Flow is the control-architecture specification standard I created at SharkNinja. It is now required on every controls project in the company. It captures the state machine, mode transitions, interrupt priorities, and safety and fault paths for a product before any firmware is written.

The weakness was never the standard, it was upkeep. The diagrams were drawn by hand, so they were expensive to produce and went stale the first time firmware changed. A diagram nobody trusts is worse than no diagram, because engineers stop reading it and start reading the code.

We moved Control Flow to **Mermaid**, using LLM-assisted generation to produce the state-machine and sequence diagrams from the control specification and the firmware itself.

**Why Mermaid**

* The diagram is **plain text**, so it lives in the repository next to the code it describes
* Changes are **reviewable in a pull request** like any other source change, instead of being an image somebody remembered to re-export
* Renders natively in **Confluence, GitHub, and Markdown**, so one source produces documentation everywhere without a drawing tool in the loop
* Cheap enough to regenerate that the diagram can be treated as **an output of the design, not a deliverable to maintain separately**

**What it changed**

* Control architecture documentation is **generated and updated as part of normal development** rather than a task deferred to the end of a program
* New engineers and offshore firmware partners onboard onto a product's control structure from a diagram that reflects current behavior
* Design reviews argue about the state machine itself instead of about whether the picture is still accurate
* Interrupt priorities, mode transitions, and safety paths stay **explicit and inspectable** on every project, which is the entire point of the standard

Internal AI-assisted product diagnostics
======

Led development of an internal tool that gives non-engineers — product managers, QA, and customer-support engineers — direct access to product-specific reasoning without going through controls engineering.

**Capabilities**

* **Natural-language questions** about how a feature works, what a control loop does, or why a given behavior might occur
* **CSV telemetry analysis** — upload unit data and get an automated first-pass diagnosis of sensor anomalies, thermal or fluid-behavior deviations, control-loop faults, and edge-case triggers
* **Grounded in team knowledge** — the tool draws on internal product documentation, historical failure modes, and engineering context, so answers are product-specific rather than generic LLM output

**Effect on the team**

* Product managers, QA, and customer-support teams self-serve the first layer of technical questions
* Controls engineers spend less time on repeated first-line diagnostics
* Issues found in the field or in QA can be triaged in hours instead of days
