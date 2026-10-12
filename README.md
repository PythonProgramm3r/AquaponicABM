# FishyGreensOS: Aquaponics & Multitrophic System Simulation (v1.1.0)

[![CoMSES Model Library](https://img.shields.io/badge/CoMSES-v1.1.0_Published-2ea44f?style=flat-square)](https://www.comses.net/codebases/07a359f3-2a04-4982-afb4-b26587274423/releases/1.1.0/)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg?style=flat-square)](https://www.gnu.org/licenses/gpl-3.0)

* **Published Model (CoMSES Computational Model Library v1.1.0):** [https://www.comses.net/codebases/07a359f3-2a04-4982-afb4-b26587274423/releases/1.1.0/](https://www.comses.net/codebases/07a359f3-2a04-4982-afb4-b26587274423/releases/1.1.0/)
* **GitHub Repository:** [https://github.com/PythonProgramm3r/AquaponicABM](https://github.com/PythonProgramm3r/AquaponicABM)
* **Empirical Input Data:** [Loyola Global Aquatic Excrement Dataset (Ecology / OSTI)](https://esajournals.onlinelibrary.wiley.com/doi/full/10.1002/ecy.1792#support-information-section)

An agent-based model built in **NetLogo** (`Aquaponic System.nlogox`) that simulates the biological resilience, nitrogen-cycle dynamics, and complex feedback loops of a closed-loop recirculating aquaponics and integrated multitrophic aquaculture (IMTA) ecosystem. Designed for agricultural research, complex systems science, and stress-testing species configurations prior to physical construction.

---

## Overview & Systemic Dynamics (v1.1.0)

This model captures the operational mechanics of a complex, sustainable production network across interconnected aquatic, bacterial, vermiculture, and hydroponic subsystems:

* **Empirical Nitrogen Cycle & Excretion Metrics:** Tracks aquatic bio-loads, bacterial nitrification, and plant nutrient uptake. Utilizing empirical biological metrics from the **Loyola Global Aquatic Excrement Dataset**, the simulation computes species-specific ammonia excretion rates (toxicity) for **Trout**, **Tilapia**, and **Goldfish** populations.
* **Bacterial Filtration & Variable Crop Uptake:** Nitrifying bacteria agents convert toxic ammonia into usable nitrates, which are absorbed at species-specific rates by **Tomato**, **Swiss Chard**, and **Lettuce** crop agents.
* **Multitrophic & Reactive Biological Buffering:** Integrates vermiculture, crawdad detritivores, and reactive biological mitigators such as emergency duckweed buffering to stabilize nutrient spikes.
* **Stochastic Environmental Shocks & Harvesting:** Stress-tests systemic resilience against chaotic environmental variables, including bio-filter pump failures, temperature crashes, and dynamic stochastic harvesting.

---

## Model Architecture & Habitats

The simulation environment models a network of specialized interconnected nodes and tank habitats:

* **Aquatic Subsystem:** Duckweed Tank, Breeding Tank, Fry Tank, Fingerling Tank, Adult Tank, and Holding Tank.
* **Bio-Filtration & Detritivore Subsystem:** Nitrifying bio-filters, vermiculture beds, and crawdad integration zones.
* **Hydroponic Grow Beds:** Variable-uptake crop beds modeling Tomato, Swiss Chard, and Lettuce growth stages and nutrient feedback penalties (toxicity or starvation).

---

## Academic Citation

> Derrick (2026, October 07). "NetLogo Aquaponic Simulation" (Version 1.1.0). *CoMSES Computational Model Library*. Retrieved from: https://www.comses.net/codebases/07a359f3-2a04-4982-afb4-b26587274423/releases/1.1.0/
