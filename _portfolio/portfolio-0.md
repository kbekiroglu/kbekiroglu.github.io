---
title: "Control Systems & Algorithm Team for Smart Products"
excerpt: "Control systems, embedded software and algorithms for SharkNinja coffee, carbonation, cooking, frozen treat, blender and Shark beauty products.<br/><img src='/images/portfolio_grid.png' width='550' height='600'>"
collection: portfolio
---

I built and run the Control Systems Engineering team at SharkNinja. We own the algorithms and embedded software in the products below, from the first prototype through mass production.

In practice that means we prototype on Raspberry Pi and Arduino with real sensors and drivers, define the state flows and the algorithms behind each feature with the embedded software engineers, build the Python and RPi rigs the validation team tests on, model the failure cases and the safe-state fallbacks, and write the specs. Most of the work is control, estimation and signal processing running on microcontrollers with very little headroom. MPC and PID, Kalman filtering, system identification, and sensor fusion across temperature, pressure and flow.

Barista Assist on the Ninja Luxe Café and Slush Assist on the frozen treat line both came out of this team.

---

## Coffee Ecosystem  
*Ninja Luxe Café, Espresso, Nespresso & Drip Machines*

- **Barista Assist Technology:** Guided brewing based on grind quality, pressure profiling, and flow curves.  
- **Milk Froth Control Algorithms:** Tuned multi-stage temperature and flow control for consistent milk texture.  
- **PID Thermal Control:** Designed high-precision espresso control loop with thermal compensation.  
- **Descaling, Jam Detection, Failures:** Embedded real-time fault detection and user alerts.

<br/><img src='/images/ninja_espresso.jpg' width='300' height='350'>

---

## Beverage & Carbonation Systems  
*Soda Machines & Cold Brew Devices*

- Developed control systems for:  
  - CO₂ level prediction & tank estimation  
  - Liquid temperature compensation  
  - Pressure release safety algorithms  
  - Dynamic state control for improved carbonation level regulation  
- Contributed to patents on carbonation accuracy and queueing logic.

<br/><img src='/images/ninja_soda.jpg' width='300' height='350'>

---

## Heated Appliances  
*Air Fryers, Indoor Grills, Ovens, Propane Grill, Slow Cookers*

- Temperature Control + Hysteresis Heater Control  
- Dynamic Temperature Offset Learning and Setpoint Adaptation  
- Sensor Fusion with NTC and Flow Sensors  
- Fast recovery and preheat tuning  
- **Smoking algorithms** for propane grill and electric grill: controlled smoke generation and thermal management across grilling modes  
- **Smart slow cooker algorithm** for adaptive long-duration cooking control  
- Extensive reliability, validation, and embedded integration.

<br/><img src='/images/ninja_grill.jpg' width='300' height='350'>

---

## Frozen Treat Makers  
*Ice Cream Makers & Slushie Machines*

- **Slush Assist Technology:**  
  - Freezing point detection  
  - Adaptive cooling energy control  
- **Temperature and compressor control for cooling systems:** precise thermal regulation and compressor duty-cycle management across freezing and hold stages  
- Adaptive cycles for varying batch sizes and consistencies.

<br/><img src='/images/ninja_icecream.jpg' width='300' height='350'>

---

## Blending & Motor Control  
*Blenders, Processors, and Mixers*

- **Blend Sense algorithm:** real-time load and consistency sensing for adaptive blending performance  
- Developed motor startup, load sensing, and failover routines  
- Created PID loops and stall protection  
- Improved safety, cycle timing, and consistency

<br/><img src='/images/ninja_blender1.jpg' width='300' height='350'>

---

## Shark Beauty Products  
*Hair Care & Skin Care Systems*

- Cross-team controls advisor to the Shark Beauty division on hair care and skin care product lines
- Contributed to controller design, tuning, and system architecture across thermal, motor, and sensing subsystems, including airflow and heat management for styling systems and thermal regulation for skin care devices
- Reviewed and debugged embedded control implementations; applied controls-theory perspective to design reviews outside my direct team's scope

<br/><img src='/images/shark_beauty.jpg' width='400' height='300'>
---
