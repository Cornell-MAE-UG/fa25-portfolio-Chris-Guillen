---
layout: project
title: Vine Vanguard, MAE 2250 Open Design Project
description: Mechanical device to crush Spotted Lanternfly egg masses at scale
technologies: [CAD, Fusion 360, 3D Printing]
image: /assets/images/SLFCrusher.png
permalink: /vine-vanguard-prototype/
---

**MAE 2250 Open Design Project** - Vine Vanguard: SLF Egg Crusher

---

### Table of Contents
- [Client Pitch](#client-pitch)
- [Functional Prototype](#functional-prototype)
- [Client Report](#client-report)

---

## Client Pitch
 
Vineyard owners across New York State face rapid *Spotted Lanternfly* (SLF) proliferation, with heavily infested vineyards reaching 400 SLF per vine. Each female lays 30-120 eggs per year, meaning populations grow exponentially. Current elimination methods (crushing masses one-by-one or applying ovicides) destroy at most 75% of eggs, and even a single surviving mass can sustain an infestation.
 
Our solution is a compact mechanical attachment that integrates with an existing scraping tool. Egg masses are scraped as normal, drop into an inlet funnel, and are immediately crushed by a rotating spiral against a fine mesh housing - no separate disposal step needed. Target users include vineyard and orchard managers, municipal forestry crews, and conservation volunteers conducting seasonal removal programs. Without effective large-scale intervention, projected losses in the Lake Erie and Finger Lakes regions alone could reach approximately $8.8 million within three years.
 
---
 
## Functional Prototype
 
The first prototype was built to test the core crushing mechanism. The assembly consists of four parts: a **spiral** (egg-shaped rotating crusher), a **spiral shaft** (hexagonal press-fit drive), an **inlet funnel** (receives egg masses from scraping), and a **mesh housing** (two-part cylinder holding the filter mesh against which eggs are crushed).
 
**What we tested and what we learned:**
 
**Press-fit structural integrity** - The shaft-spiral and funnel-housing connections seated securely. However, the housing top and bottom tolerances were inaccurate and required duct tape to hold together. When inverted during the shake test, the shaft and spiral slid freely out of the housing bottom. Next iteration will revise CAD tolerances and add a retention feature.
 
**Spiral rotation under load** - Rotation was smooth with no load. Under simulated egg masses (hydrated Orbeez), eggs lodged beneath the spiral rather than passing through the crushing zone, causing intermittent jamming. The temporary mesh used for testing had ~8mm openings versus 3mm Orbeez, so eggs fell through instead of being crushed. Next iteration will add interior guide arms to keep the spiral flush against the mesh bottom, and replace the temporary mesh with fine mesh sized below egg diameter.
 
**Crushing efficiency** - Quantitative efficiency could not be measured due to the mesh sizing issue. Qualitatively, the spiral's tapered base allowed eggs to accumulate at the housing bottom with no way to clear them, and the mesh showed instability under lateral load. Next iteration will redesign the spiral to not taper inward at the base and will explore more secure mesh configurations.
 
**Success criteria for the final prototype:**
- ≥ 80% of eggs crushed per mass
- Processing rate of 2-3 eggs per second (to be tested once motor is integrated)
- Device bounding box ≤ 6 x 6 x 10 inches, weight ≤ 4 lbs

---

## Client Report

[Download Full Report (PDF)]({{ "/assets/ODP_6_Client_Report_Finallllll.pdf" | relative_url }}){:target="_blank"}

### Project Overview

The Vine Vanguard egg crusher is a juicer-inspired mechanical device designed to destroy Spotted Lanternfly (SLF) egg masses at scale. The device works by dropping scraped egg masses into an inlet funnel, where a motor-driven rotating spiral presses them against the interior surface of a fine mesh cylinder-crushing eggs and expelling debris through the mesh. The goal was to develop and test a functional prototype within a $350 budget that meets or exceeds ≥ 80% crushing efficiency.

**Prototype cost: $195.56, well within the $350 budget.**

---

### Final Prototype Design

The second-iteration prototype addressed all issues identified in O5 testing. Key design changes:

- **Spiral geometry revised** - removed the inward taper at the base so eggs cannot accumulate beneath the spiral; new profile maintains consistent contact with the mesh wall throughout the full spiral length
- **Guide arms added** - three interior arms keep the spiral flush against the mesh bottom, eliminating the jamming behavior observed with Orbeez-sized objects
- **Mesh replaced** - temporary large-opening mesh swapped for fine mesh sized below SLF egg diameter (~0.5 mm openings), ensuring eggs are crushed rather than falling through
- **Housing tolerances corrected** - top/bottom housing fits revised in CAD; no tape required; retention feature added so the shaft-spiral assembly cannot slide out when inverted

---

### Testing & Results

Testing was conducted using real SLF egg masses collected during the season. Each trial recorded number of eggs input, eggs visibly crushed (passed through or pressed flat against mesh), and structural outcomes.

| Metric | Result |
|---|---|
| Crushing efficiency (avg.) | **~80%** |
| Failure rate (standard egg mass) | **0%** |
| Optimal batch size | **30-50 eggs (1 egg mass)** |
| Prototype cost | **$195.56 / $350 budget** |

**Key findings:**

- At 30-50 eggs (a single standard egg mass), the spiral maintained consistent contact across the full mesh surface and achieved ~80% throughput with no jams.
- Above ~80 eggs, eggs began stacking above the active crushing zone, reducing efficiency. A series-crushing mechanism (multiple passes or a multi-stage spiral) would address this.
- Below 10 eggs, the device operated cleanly but underutilized-acceptable given real-world egg masses cluster in the 30-50 range.
- No structural failures were recorded across all test runs: housing held without fasteners, shaft retained under inversion, and mesh maintained integrity after repeated crush cycles.

---

### Recommendations for Future Development

| Priority | Recommendation |
|---|---|
| High | **Spiral geometry optimization** - iteratively vary spiral pitch and taper to push efficiency beyond 80% and expand the optimal batch range |
| High | **Compactness** - reduce overall bounding box; current prototype exceeds the 6 x 6 x 10 in. target and would benefit from a shorter housing and integrated motor mount |
| Medium | **Series crushing mechanism** - add a second pass or multi-stage spiral to handle larger batch sizes (80+ eggs) without loss of efficiency |
| Medium | **Motor integration** - current testing used manual rotation; a corded or battery motor must be selected and mounted before field trials |
| Low | **Ergonomics & attachment interface** - finalize the scraper-attachment geometry so the device clips onto standard vineyard scraping tools |

---

### Conclusion

The Vine Vanguard prototype demonstrates that a rotating-spiral-against-mesh mechanism is a viable approach to large-scale SLF egg mass destruction. The ~80% crushing efficiency at the target batch size of 30-50 eggs meets the project success criterion, and the 0% structural failure rate confirms the revised CAD tolerances are sound. The device was delivered within budget at $195.56.

The core mechanism is proven. Future iterations should focus on geometry optimization and compactness to make the device practical for seasonal field use by vineyard and orchard managers.