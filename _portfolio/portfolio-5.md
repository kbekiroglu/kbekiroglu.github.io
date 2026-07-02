---
title: "Real-Time R&D Data Collection Platform"
excerpt: "Built the internal Python/Serial data-collection GUI and sensor profiler used across SharkNinja beverage and heated-product R&D — real-time MCU communication, CSV logging, live plotting. Early SharkNinja project (Senior Systems Engineer, 2022); still used across product lines today.<br/><img src='/images/serialGUI.png' width='550' height='600'><br/><br/><img src='/images/profiler2.jpg' width='400' height='450'>"
collection: portfolio
---

Early SharkNinja project built as Senior Systems Engineer (2022): a Python-based data-collection GUI and a sensor/scale profiler for beverage and heated-product R&D. Both are still used across the Control Systems team today.

Serial GUI — MCU Data Collection
======

Python application that opens a serial link (UART / USB serial) to the product's microcontroller and provides:

* **Telemetry ingestion** from MCU firmware and auxiliary validation sensors
* **Two-way command interface** — trigger actuators, change setpoints, and drive test sequences directly from the GUI
* **CSV logging** with per-channel timestamps for offline analysis
* **Live plotting** of multiple sensor channels for identifying trends, transients, and anomalies during HIL testing

Purpose: eliminate manual instrumentation and data-manipulation overhead so R&D and test engineers iterate on algorithms and firmware without stopping to wrangle data.

Sensor & Scale Profiler
======

Companion tool for R&D and test teams to visualize, timestamp, and save sensor and scale data during characterization runs: pressure, temperature, flow, and load-cell readings streamed into a synchronized profile that can be replayed, compared, and exported.

Both tools became standard R&D infrastructure across the coffee, carbonation, and thermal-cooking product lines.

