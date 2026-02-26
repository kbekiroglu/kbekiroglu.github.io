---
title: "Robust MPC design / Robust intervention and Robust Optimization"
excerpt: "Robust MPC design / Robust intervention and Robust optimization methods are developed and used in the behavioural intervention design.<br/><img src='/images/smoking.jpg'>"
collection: portfolio
---

The clinical and behavioral scientist has some techniques that use non-intensive behavioral data to develop adaptive treatment algorithms. Using non-intensive data is because collecting intensive longitudinal data was challenging before recent developments on portable devices such as mobile phones. With the advent of such devices, collecting many measurements over time is effortless since patients can easily be reached. This study explains how control engineering methods can be adapted to handle most of the challenges that come from the structure of the intensive longitudinal data while effectively using portable devices. We aim to introduce procedures that utilize available patients' data to develop algorithms that determine the next steps in an individual's treatment.
<br/><img src='/images/rcontrol.jpg'>

Steps in Behavioural Intervention Design:
------
* Step 1: Decide on message frequency (Assume contact patient three times).
* Step 2: The patient provides information on his/her measurements of smoking urge (1), negative effect (1), self-efficacy (1), Treatment (1) in the morning.
* Step 3: At midday, the message collects smoking urge (2), negative effect (2), and self-efficacy (2).
* Step 4: Build measurement set M (e.g., at midday, it has smoking urge (1), negative effect (1), self-efficacy (1), Treatment (1), smoking urge (2), negative effect (2), and self-efficacy (2)
* Step 5: Run the MPC algorithm with identified model f, calculate TOptimal, update measurement set M, and message Treatment (2) = TOptimal to the patient.
* Step 6: Collect new state values smoking urge (3), negative effect (3), and self-efficacy (3) in the evening and update measurement set M.
* Step 7: Repeat this process throughout the entire process of treatment.

