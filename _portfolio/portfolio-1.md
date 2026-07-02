---
title: "AI-Assisted Engineering — Adoption and Internal AI Tooling"
excerpt: "Drove Claude Code and OpenAI Codex adoption across the SharkNinja Control Systems team. Same headcount now supports approximately 40% more concurrent projects. Also led an internal AI diagnostic tool that lets non-engineers ask product questions and analyze CSV telemetry to identify software or hardware issues."
collection: portfolio
---

As Senior Director of Control Systems Engineering, I lead two AI initiatives at SharkNinja: standardizing LLM-assisted workflows across the engineering team, and building an internal AI diagnostic tool that lets non-engineers reason about product behavior directly from unit telemetry.

Impact
======

* Same engineering headcount supports approximately **40% more concurrent projects**
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
