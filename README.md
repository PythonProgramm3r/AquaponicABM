# FishyGreensOS: Aquaponics & Multitrophic System Simulation

An agent-based model built in NetLogo[cite: 1] that simulates a closed-loop recirculating aquaponics and integrated multitrophic aquaculture (IMTA) ecosystem, modeling the complex dynamics between aquatic species, vermaculture, and hydroponic plant beds[cite: 1].

## Overview

This model captures the operational mechanics of a complex, sustainable production network[cite: 1]. It tracks nutrient flows, water recirculation pathways, biological growth stages, and environmental feedback penalties (such as nutrient toxicity or starvation) across multiple specialized tanks and grow beds[cite: 1].

## Model Architecture & Habitats

The simulation environment models a network of distinct interconnected nodes and tank habitats[cite: 1]:
* **Aquatic Subsystem:** Duckweed Tank, Breeding Tank, Fry Tank, Fingerling Tank, Adult Tank, and a Holding Tank for harvested fish[cite: 1].
* **Benthic & Waste Management:** Crawdad Tank 1 & 2 for bottom-feeding and waste processing, alongside a Vermaculture node populated by composting worms[cite: 1].
* **Hydroponic Subsystem:** Five sequential Grow Beds and a recirculating loop feeding back into the system[cite: 1].

## Key Agent Dynamics

* **Water Flow Visualization:** Active links between tanks spawn animated `droplet` agents that visually simulate recirculating water dynamics across the network[cite: 1].
* **Biological Growth & Aging:** Fish and plants progress through age-based development thresholds governed by species-specific parameters[cite: 1]. 
* **Feedback Loops:** 
  * *Toxicity Penalty:* Excess nutrients (`nutrient-per-day > 80`) slow fish growth rates by 50%[cite: 1].
  * *Starvation Penalty:* Insufficient nutrient levels (`nutrient-per-day < 30`) delay plant maturation by 50%[cite: 1].

## Interface Controls

* **`fish-type` Chooser:** Selects the primary aquatic species (Tilapia, Channel Catfish, Trout, Goldfish), altering base growth thresholds[cite: 1].
* **`plant-type` Chooser:** Selects the cultivated crop (Lettuce, Basil, Tomatoes, Mint)[cite: 1].
* **`nutrient-per-day` Slider:** Manages daily nutrient input to balance system load and avoid toxicity or starvation thresholds[cite: 1].
* **Dashboard Plot:** Real-time tracking of `total-fish-harvested` and `total-plants-harvested`[cite: 1].

## Getting Started

1. Download and install [NetLogo 7.0+](https://ccl.northwestern.edu/netlogo/)[cite: 1].
2. Clone this repository or download the `.nlogo` model file[cite: 1].
3. Open the file in NetLogo, click **setup** to initialize the tank network and biological populations, and click **go** to run the simulation[cite: 1].
