---
title: "From 3D groundwater simulations to regional groundwater heat pump potential"
author: "Emanuel Huber"
date: "2026"
description: "LinkedIn article based on Huber, Badoux & Lützenkirchen (2026)"
---

# From 3D groundwater simulations to regional groundwater heat pump potential

How can we estimate how many groundwater heat pump systems can be installed in an entire aquifer while accounting for thermal interference between systems?

This was the central question behind our recent study:

**“Quantifying the permissible technical groundwater heat pump potential and its uncertainty through aquifer clustering and spatial packing.”**

[Read the paper](https://doi.org/10.1007/s00767-025-00609-9)

## The challenge

Groundwater heat pump (GWHP) systems are inherently three-dimensional. A single installation can modify groundwater temperature over a considerable distance, and when several systems are installed close to each other, their thermal influence zones interact.

At the same time, running a detailed 3D groundwater-flow and heat-transport simulation for every possible installation across a regional aquifer is computationally impractical.

We therefore developed a different approach.

## The basic idea

The central concept is to separate the problem into two levels.

At the first level, we retain detailed physics: representative GWHP configurations are simulated with 3D groundwater-flow and heat-transport models.

At the second level, the results of these simulations are converted into spatial influence zones that can be used for regional planning.

The workflow is:

**Aquifer → clustering → representative 3D simulations → influence zones → spatial packing → regional potential**

## 1. Cluster the aquifer

The aquifer is divided into representative hydrogeological clusters using parameters such as:

- hydraulic conductivity
- groundwater thickness
- hydraulic gradient

For each cluster, representative hydrogeological properties are extracted.

This reduces the number of expensive numerical simulations while retaining the main spatial variability of the aquifer.

## 2. Simulate representative GWHP systems

For each cluster, a GWHP doublet is simulated using a 3D groundwater-flow and heat-transport box model.

The study considers three energy-demand profiles, with both balanced and unbalanced energy loads, over a 20-year operating period.

The simulations account for groundwater flow, heat transport and thermal influence around the doublet.

## 3. Convert simulations into influence zones

The detailed numerical results are then transformed into spatial influence zones.

The influence zone combines the thermal plume, represented using a 0.1 K isotherm, with a hydraulic criterion based on the Darcy velocity relative to the natural groundwater flow.

This is an important step.

The result of an expensive numerical simulation becomes a reusable spatial object.

Instead of repeatedly running the full 3D model, we can use these influence zones to investigate many possible installation configurations.

## 4. Pack the influence zones across the aquifer

The influence zones are then spatially packed within the hydrogeological clusters.

The packing respects three main constraints:

1. influence zones cannot overlap;
2. systems must remain associated with their hydrogeological cluster;
3. the systems are aligned with the groundwater-flow direction.

The maximum number of non-overlapping influence zones provides the basis for estimating the permissible technical GWHP potential.

Conceptually:

**expensive numerical physics**

↓

**representative simulations**

↓

**spatial influence zones**

↓

**regional spatial planning**

## 5. Quantify uncertainty

The assessment is not reduced to a single deterministic number.

Hydrogeological variability is represented by subclusters, and an additional simulation is performed with a 6° deviation from the natural groundwater-flow direction.

The smallest and largest resulting influence zones are then used in the packing procedure to estimate a range of possible technical potential.

This provides a scenario-based representation of uncertainty rather than treating the potential as a single exact value.

## Application to the Baar–Zug–Steinhausen aquifer

The methodology was applied to the deep aquifer in the Baar–Zug–Steinhausen area in the canton of Zug, Switzerland.

The aquifer extends over approximately 10 km² and occurs at depths of roughly 80–230 m. The investigation used available hydrogeological information because no regional groundwater model was available.

![Study area and aquifer](https://media.springernature.com/full/springer-static/image/art%3A10.1007%2Fs00767-025-00609-9/MediaObjects/767_2025_609_Fig1_HTML.png)

*Figure 1 from Huber, Badoux & Lützenkirchen (2026): study perimeter, groundwater heads and aquifer thickness.*

## What does the study show?

The results demonstrate that the deep aquifer has substantial technical potential for groundwater heat pump applications.

Several findings are particularly relevant:

- The estimated potential depends strongly on the hydrogeological setting and the spatial interaction between systems.
- Balanced energy-load profiles generally allow more efficient use of the available aquifer space than unbalanced profiles.
- Larger GWHP systems can be more space-efficient because each installation can satisfy a larger energy demand.
- The size and shape of thermal influence zones vary substantially between hydrogeological clusters.
- Uncertainty is particularly relevant in clusters with higher groundwater velocities and greater hydrogeological variability.
- In all simulated cases, the temperature change 100 m downstream of the reinjection point remained below the 3 K regulatory criterion used in the study.

The simulations showed maximum temperature changes below 1.51 K at that distance, indicating that the tested 375 kW systems remained below the regulatory temperature-change limit.

## What I consider the main contribution

The main contribution is not a single potential value for one Swiss aquifer.

It is the **framework for scaling detailed 3D simulations to regional assessments**.

A limited number of physically detailed simulations can be converted into reusable spatial representations of their influence. These representations can then be combined with a spatial packing algorithm to explore regional installation potential.

This provides a bridge between:

**local, detailed numerical modelling**

and

**regional geothermal planning.**

## The influence zones

One of the most informative results is the variation of the influence zones between hydrogeological clusters and energy-load profiles.

![Influence zones](https://media.springernature.com/full/springer-static/image/art%3A10.1007%2Fs00767-025-00609-9/MediaObjects/767_2025_609_Fig3_HTML.png)

*Figure 3 from the paper: influence zones for the different hydrogeological clusters and energy-load profiles.*

The figure illustrates why a simple rule such as “one installation per X square metres” is not sufficient.

The spatial footprint of a GWHP system depends on the groundwater flow regime, aquifer properties and operating conditions.

## From influence zones to regional potential

The next step is to place these influence zones across the aquifer while preventing overlap.

![Spatial packing](https://media.springernature.com/full/springer-static/image/art%3A10.1007%2Fs00767-025-00609-9/MediaObjects/767_2025_609_Fig5_HTML.png)

*Figure 5 from the paper: example of the spatial packing of GWHP influence zones.*

This is where the approach changes from a conventional numerical-modelling problem into a spatial-planning problem.

The numerical model provides the physically meaningful building blocks.

The packing algorithm determines how many of these building blocks can coexist.

## How different operating conditions affect the result

The simulations also show how influence-zone length and heat-recovery efficiency vary with hydrogeological cluster, energy-load profile and operating mode.

![Influence-zone length and heat recovery](https://media.springernature.com/full/springer-static/image/art%3A10.1007%2Fs00767-025-00609-9/MediaObjects/767_2025_609_Fig4_HTML.png)

*Figure 4 from the paper: influence-zone length and heat-recovery efficiency for the investigated clusters and operating conditions.*

For the investigated configurations, recirculative systems generally showed lower heat-recovery efficiencies, while bidirectional systems benefited more from the thermal memory of the aquifer.

The exact behaviour depends on the hydrogeological setting and operating conditions.

## Why could this approach be useful beyond this case study?

The same general concept could potentially be investigated for other problems where detailed numerical simulations are expensive but regional spatial planning is required.

Examples include:

- groundwater heating and cooling;
- aquifer thermal energy storage;
- geothermal well spacing;
- thermal interference between installations;
- regional geothermal planning;
- other applications where simulation results can be represented as spatial constraints.

The important idea is therefore broader than a particular algorithm or a particular aquifer:

> **Use detailed numerical models where physics matters most, then reuse their results as spatial representations for large-scale planning.**

## What comes next?

There are several directions for further development.

One important step would be to systematically compare the reduced approach with a much larger number of full 3D simulations and quantify the approximation error.

Other questions include:

- How many hydrogeological clusters are needed?
- How sensitive is the estimated potential to the clustering method?
- How should heterogeneous aquifer properties be represented?
- How can spatially variable groundwater flow directions be handled?
- How accurately can influence zones represent interactions between multiple systems?
- Can the same framework be combined with more advanced optimization methods?

These questions could help move from a case-study methodology towards a more general computational framework for regional geothermal planning.

## Reference

Huber, E., Badoux, V. & Lützenkirchen, V. (2026). *Quantifying the permissible technical groundwater heat pump potential and its uncertainty through aquifer clustering and spatial packing*. **Grundwasser**, 31, 33–46.

https://doi.org/10.1007/s00767-025-00609-9

---

## Recommended figures for LinkedIn

For a LinkedIn publication, I would **not use all figures**.

### 1. Main / hero figure: Figure 5 — spatial packing

This is the strongest visual representation of the originality of the approach. It shows the transition from individual simulated influence zones to regional potential.

### 2. Supporting figure: Figure 3 — influence zones

This explains the physical basis of the spatial packing and makes the hydrogeological variability visible.

### 3. Context figure: Figure 1 — study area

Useful if you want to show where the case study is located, but it is less important for communicating the methodological novelty.

### 4. Optional results figure: Figure 4

Useful if you want the article to emphasize the comparison between operating modes, influence-zone size and heat-recovery efficiency.

### My recommended LinkedIn sequence

**Cover:** Figure 5  
→ short explanation of the problem

**Figure 3:**  
→ explain why influence zones differ

**Figure 5 again or a cropped/high-resolution version:**  
→ explain spatial packing

**Figure 4:**  
→ show the physical results

I would avoid making Figure 1 the first image. It communicates the study site, but **Figure 5 communicates the idea**.
