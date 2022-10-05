---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* B.S. in in Electrical and Electronics Engineering, Karadeniz Technical University, Trabzon, Turkey, 2005
* M.S. in Electrical and Computer Engineering, Northeastern University, Boston, MA, 2010
* Ph.D in Electrical Engineering, The Pennsylvania State University, University Park, PA, 2015
  * Minor Ph.D in Industrial and Manufacturing Engineering (Convex Optimization), The Pennsylvania State University, University Park, PA, 2015

* MOOC Certificates
  * Coursera: Fundamentals of Scalable Data Science by IBM- May 2019
  * Coursera: Neural Networks and Deep Learning by deeplearning.ai - June 2019

Work experience
======
* 12/2021 to Present: Senior System Engineer, SharkNinja
  * Conceptualized/Designed/Implemented various signal processing/sensing tools and controllers for Ninja Heated products. 
    * Successfully developed control systems (e.g., cascade temperature control, flow control) and algorithms (e.g., failure detection, altitude calibration, low pass filter) for all features of one Ninja Coffee Machine in the market. From prototype development to mass production, algorithms were developed (in C++, Arduino, and Python) and implemented in the final product.
    * Owned/Managed the prototype and testing tools development. A Python application and an R-pi/Arduino apparatus were developed to speed up the testing process.

* 08/2019 to Present: Co-founder, [Ocean Dynamex](https://www.oceandynamex.com/)
  * Supporting the industry with predictive workflow systems, mathematical modeling, algorithmic systems, and control engineering. The company is also developing new forecasting software to support the maritime industry.
    * Successfully developed and tested a new mathematical grid search algorithm ([IMSE](https://www.sciencedirect.com/science/article/abs/pii/S0306261918311000)) and an [ensemble learning](https://www.sciencedirect.com/science/article/abs/pii/S0950705121011059) forecasting method for various industries' forecasting problems.
    * Compared our new algorithm with benchmark methods and proved its performance.
* 08/2018 to 12/2021: Researcher, SUNY Poly - Assistant Prof.
  * Led various mathematical modeling, model predictive controller design, and IoT research projects. Developed an (IoT) based pavement monitoring system for a transportation agency. Researched/Evaluated the real-time implementation challenges in computer network anomaly detection and artificial pancreas MPC design.  
    * [A low-cost IoT-based](https://ieeexplore.ieee.org/abstract/document/9694224) (R-pi and AWS are used) wireless online structural monitoring/data collection system of asphalt has been developed.
    * AP design for type-2 diabetes: Data collection was performed, and a personal modeling method was evolved for MPC design. Also, behavioral intervention by using MPC was implemented to support patients in real time.
    * A new optimization-based combined forecasting method was developed and tested in two different data sets (tourist number and crude oil price). Results were compared with benchmark methods. 
* 12/2016 to 08/2018: Research Engineer, Nanyang Technological University
  * A scalable, energy-saving solution for commercial buildings' HVAC systems was successfully developed and implemented on the Nanyang Technological University campus. A distributed MPC solution and its implementation were deployed on top of the existing HVAC system through an IoT network. 
    * [Distributed MPC design for HVAC systems](https://www.sciencedirect.com/science/article/abs/pii/S0306261919302582) were deployed in a commercial building (Nonlinear MPC using MATLAB in server and Linear MPC using Python in R-pi). 
    * On average, 12-13% energy saving was obtained in real-time testing.
    * Real-time room temperature model learning is created to support local MPC.
* 08/2015 to 12/2016: Researcher, The Methodology Center – Penn State University 
  * Used MPC to design an intervention for smoking study.
  * Researched/Developed/Implemented robust MPC for bounded uncertainties to diminish the craving.
  * Generated project deliverables based on the insights from the data and developed algorithms.
* 09/2010 to 12/2015: Research Assistant, Pennsylvania State University - University Park
  * Smart Treatment for Behavioral Problems: From Data to Controllers: Using system identification and robust control to design effective treatments.
  * Randomized Algorithms for System Identification: From data to linear/non-linear models. Average model from population data. Developed a mathematical model for smoking cravings.
* 09/2008 to 08/2010: Research Assistant, Northeastern University - Boston
  * Developed UAV using computer vision algorithms and PID controller to track a predefined target.
  * Image tracking in real-time as feedback to the controller for reference tracking. 
                                              
Skills
======
* Hard Skills
  * MPC design
  * Robust MPC
  * Optimization
  * Mechatronic design
  * Non-linear Programming 
  * System Identification
  * IoT in control
  * Signal processing
  * Time-series analysis
  * Predictive analytic
  * Building Automation
  * Filtering Design
* Languages
  * Python
  * MATLAB
  * Simulink
  * Energy Plus
  * Arduino
* Tools
  * CVX
  * YALMIP
  * CPLEX
  * Mosek
  * Gurobi
* Soft Skills
  * Mentored graduate and undergraduate students, collaborating with engineers/scientists from various fields, initiated, organized, and led a team for an IoT project, and prepared a final technical report.

Publications
======
  <ul>{% for post in site.publications %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Talks
======
  <ul>{% for post in site.talks %}
    {% include archive-single-talk-cv.html %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
# Service and leadership
# ======
# * Currently signed in to 43 different slack teams
