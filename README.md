# FishyGreensOS: Aquaponics & Multitrophic System Simulation

An agent-based model built in NetLogo that simulates a closed-loop recirculating aquaponics and integrated multitrophic aquaculture (IMTA) ecosystem, modeling the complex dynamics between aquatic species, vermaculture, and hydroponic plant beds.

## Overview

This model captures the operational mechanics of a complex, sustainable production network. It tracks nutrient flows, water recirculation pathways, biological growth stages, and environmental feedback penalties (such as nutrient toxicity or starvation) across multiple specialized tanks and grow beds.

## Model Architecture & Habitats

The simulation environment models a network of distinct interconnected nodes and tank habitats:
* **Aquatic Subsystem:** Duckweed Tank, Breeding Tank, Fry Tank, Fingerling Tank, Adult Tank, and a Holding Tank for harvested fish.
* **Benthic & Waste Management:** Crawdad Tank 1 & 2 for bottom-feeding and waste processing, alongside a Vermaculture node populated by composting worms.
* **Hydroponic Subsystem:** Five sequential Grow Beds and a recirculating loop feeding back into the system.

## Key Agent Dynamics

* **Water Flow Visualization:** Active links between tanks spawn animated `droplet` agents that visually simulate recirculating water dynamics across the network.
* **Biological Growth & Aging:** Fish and plants progress through age-based development thresholds governed by species-specific parameters. 
* **Feedback Loops:** 
  * *Toxicity Penalty:* Excess nutrients (`nutrient-per-day > 80`) slow fish growth rates by 50%.
  * *Starvation Penalty:* Insufficient nutrient levels (`nutrient-per-day < 30`) delay plant maturation by 50%.

## Interface Controls

* **`fish-type` Chooser:** Selects the primary aquatic species (Tilapia, Channel Catfish, Trout, Goldfish), altering base growth thresholds.
* **`plant-type` Chooser:** Selects the cultivated crop (Lettuce, Basil, Tomatoes, Mint).
* **`nutrient-per-day` Slider:** Manages daily nutrient input to balance system load and avoid toxicity or starvation thresholds.
* **Dashboard Plot:** Real-time tracking of `total-fish-harvested` and `total-plants-harvested`.

## Getting Started

1. Download and install [NetLogo 7.0+](https://ccl.northwestern.edu/netlogo/).
2. Clone this repository or download the `.nlogo` model file.
3. Open the file in NetLogo, click **setup** to initialize the tank network and biological populations, and click **go** to run the simulation.
