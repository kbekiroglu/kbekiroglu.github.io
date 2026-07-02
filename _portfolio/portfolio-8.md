---
title: "System Identification & Mathematical Modeling — PhD Research"
excerpt: "PhD dissertation research at Penn State (2010–2015): sparse and randomized system identification algorithms for noisy, incomplete data, with applied deployments across behavioral health, radar tracking, thermal modeling, and forecasting.<br/><img src='/images/sparse.jpg'>"
collection: portfolio
---

PhD dissertation research at **The Pennsylvania State University (2010–2015)**: [*From Data to Interventions: Using System Identification and Robust Control Algorithms to Design Effective Treatments*](https://etda.libraries.psu.edu/catalog/26227). Advisor: Prof. Constantino Lagoa. Collaborator: Prof. Mario Sznaier (Northeastern). The dissertation developed randomized and atomic-norm-based algorithms for parsimonious system identification, recovering low-order models from noisy and incomplete data. The line of work extended through postdoctoral and faculty roles into new domains.

Theoretical foundations
======

* **Randomized algorithm for parsimonious model identification** — atomic-norm minimization for low-order model recovery from noisy data ([IEEE Trans. Automatic Control, 2017](https://ieeexplore.ieee.org/document/7970196))
* **Low-order MIMO identification from noisy, incomplete data** ([54th IEEE CDC, 2015](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=7402846))
* **Parsimonious model identification via atomic norm minimization** ([European Control Conference, 2014](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=6862636))
* **Recursive parsimonious system identification** for dynamical systems ([IEEE CCTA, 2018](https://ieeexplore.ieee.org/abstract/document/8511460))
* **Parsimonious Volterra system identification** for nonlinear systems ([IEEE ACC, 2018](https://ieeexplore.ieee.org/document/8431084))

Applied deployments
======

* **Behavioral health interventions** — control-theoretic methods applied to smoking cessation, physical activity, and adaptive treatment design ([IEEE Trans. Control Systems Technology, 2016](https://ieeexplore.ieee.org/ielaam/87/7876877/7501575-aam.pdf); [Drug & Alcohol Dependence, 2017](https://www.sciencedirect.com/science/article/abs/pii/S0376871617304234); [Int. Journal of Control, 2021](https://www.tandfonline.com/journals/tcon20); [Journal of Consulting & Clinical Psychology, 2014](https://psycnet.apa.org/record/2014-27336-001)). See **worked example below** for the intervention loop.
* **Bearing-only tracking for passive radar** — Hankel matrix rank as an indicator of ghost targets ([IEEE Trans. Aerospace & Electronic Systems, 2018](https://ieeexplore.ieee.org/document/8340803))
* **Thermal dynamical modeling** for smart buildings — recursive online identification for adaptive HVAC control ([IEEE/CAA Journal of Automatica Sinica, 2020](https://ieeexplore.ieee.org/abstract/document/9080611)) <br/><img src='/images/sysid.png'>
* **Time-series forecasting** — multi-method combined-forecast algorithm ([Knowledge-Based Systems, 2022](https://www.sciencedirect.com/science/article/pii/S0950705121011059))
* **Material testing and classification** — model-order validation and noise reduction for impact-resonance testing of asphalt concrete ([Journal of Nondestructive Evaluation, 2017](https://link.springer.com/article/10.1007/s10921-017-0436-2))

Full publication list on [Google Scholar](https://scholar.google.com.sg/citations?hl=en&user=pely-qQAAAAJ).

<br/>

Worked example — Robust MPC for behavioral intervention design
======

<br/><img src='/images/smoking.jpg'>

Application of the theory to smoking cessation and adaptive behavioral treatment. Traditional clinical practice relied on non-intensive behavioral data because collecting intensive longitudinal data was impractical. Mobile devices make intensive per-patient measurements feasible, and the resulting data (short samples, high noise, missing entries) fits the parsimonious identification and robust MPC methods above. The algorithm below determines the next intervention step from patient self-report data in real time ([IEEE CDC, 2013](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=6760421); [IEEE CCA, 2016](http://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=7587951)).

<br/><img src='/images/rcontrol.jpg'>

**Intervention loop (three contacts per day):**

1. Decide on message frequency — three contacts per day for this example
2. **Morning:** patient reports smoking urge (1), negative affect (1), self-efficacy (1), and prior treatment (1)
3. **Midday:** collect smoking urge (2), negative affect (2), self-efficacy (2)
4. Build measurement set *M* — accumulate all readings collected so far in the day
5. Run the **robust MPC algorithm** with the identified patient-dynamics model *f*, compute *T*<sub>optimal</sub>, update *M*, and message the next treatment step to the patient
6. **Evening:** collect smoking urge (3), negative affect (3), self-efficacy (3); update *M*
7. Repeat throughout the entire course of treatment — the patient-specific model *f* is re-identified online as new data arrives

