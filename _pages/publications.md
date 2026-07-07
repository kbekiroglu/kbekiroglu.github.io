---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if site.author.googlescholar %}
  Full list on <u><a href="{{ site.author.googlescholar }}">Google Scholar</a></u> (40+ publications).
{% endif %}

{% include base_path %}

## Selected Publications

**Control & System Identification**

- **A Randomized Algorithm for Parsimonious Model Identification.** *IEEE Transactions on Automatic Control*, 2017. Yılmaz, Bekiroglu, Lagoa, Sznaier. [[paper](https://ieeexplore.ieee.org/document/7970196)]
- **Control Engineering Methods for the Design of Robust Behavioral Treatments.** *IEEE Transactions on Control Systems Technology*, 2017. Bekiroglu, Lagoa, Murphy, Lanza. [[paper](https://ieeexplore.ieee.org/ielaam/87/7876877/7501575-aam.pdf)]
- **Recursive approximation of complex behaviours with IoT-data imperfections.** *IEEE/CAA Journal of Automatica Sinica*, 2020. Bekiroglu, Srinivasan, Png, Su, Lagoa. [[paper](https://ieeexplore.ieee.org/abstract/document/9080611)]

**Robotics & Vision-Based Control**

- **Computer Vision Based Control of an Autonomous Blimp.** *Turkish Journal of Electrical Engineering & Computer Sciences*, 2016. Bekiroglu, Sznaier, Lagoa, Shafai. [[paper](https://journals.tubitak.gov.tr/cgi/viewcontent.cgi?article=2548&context=elektrik)]

**Estimation & Tracking**

- **Hankel Matrix Rank as Indicator of Ghost in Bearing-Only Tracking.** *IEEE Transactions on Aerospace and Electronic Systems*, 2018. Bekiroglu, Ayazoglu, Lagoa, Sznaier. [[paper](https://ieeexplore.ieee.org/document/8340803)]

**Applied MPC & IoT**

- **An IoT Upgrade for Smart and Scalable HVAC Control in Commercial Buildings.** *Applied Energy*, 2019. Png, Srinivasan, **Bekiroglu**, Chaoyang, Su, Poolla. **162 citations.** [[paper](https://www.sciencedirect.com/science/article/abs/pii/S0306261919302582)]

---

## All Publications

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
