---
layout: project
title: Virtual Fencing
description: GPS-based virtual boundary system + iterative ear-tag CAD + electric stimuli prototyping
technologies: [Fusion360, BantamTools, ANSYS]
image: /assets/images/virtual-fencing/design-process.JPEG
---

**Overview**  

Virtual fencing is a livestock management approach that uses GPS tracking and stimuli (sound + electric shock) to keep animals within a farmer-defined virtual boundary. Instead of physically moving fences, farmers can set GPS coordinates and track animals in real time, with collars (or tags) by triggering a stimuli as animals approach the boundary.

---

**Problem + Motivation**

Traditional fencing requires significant time and labor to manage, and for large-scale farms the maintenance costs can be substantial. Although virtual fencing systems exist, they are often prohibitively expensive and depend on bulky, heavy collars that introduce snagging and usability concerns.

---

**Project Goal**

Our team was tasked with designing an affordable, low-cost cow ear tag alternative that reduces size compared to traditional collars and makes virtual fencing more accessible, particularly in low- and middle-income countries. The goal was to monitor cow movement and behavior using sensor data (GPS and accelerometer) and apply electric and visual/sound-based stimuli to deter boundary crossing.

---

**Customer Discovery (what we learned from farmers / stakeholders)**  

Key concerns raised during customer discovery included cost, communication and reliability (such as Wi-Fi connectivity issues), and overall trust in the system. Farmers also emphasized the need for fencing flexibility across seasons, with larger grazing areas in the summer and smaller ones in the winter. While traditional and electric fencing are widely used, they present ongoing challenges related to maintaining electrical charge, long-term durability, and physical upkeep, including wires being damaged by branches or terrain.

When asked what would motivate them to invest in a new system, farmers consistently cited being driven by necessity and the importance of a solution that is both cost-effective and highly reliable.

---

**My Contribution (Jamison — CAD + Iteration)**  

I designed and iterated on electronic enclosures in Fusion 360, with a focus on safety, animal comfort, and cost-effective deployment for farmers in low- and middle-income regions. To validate and refine the design, I conducted 24 finite element analysis (FEA) simulations in ANSYS and Fusion 360, evaluating factor of safety, material strength, and material efficiency by modeling realistic loading conditions ranging from a cow chewing on the enclosure at 200 N to full biting forces of 800 N. In parallel, I performed on-farm testing using different enclosure materials—Nylon 66, Nylon 6, and PLA—to identify an ideal prototyping material that balanced durability, manufacturability, and performance.

<figure style="width:400px; margin:0 auto; text-align:center;">
  <img src="{{ "/assets/images/virtual-fencing/fea-graphs.pdf" | relative_url }}"
       alt="Finite Element Analysis of Enclosure 1a and 1b"
       style="display:block; width:100%; margin:0 auto;">
  <figcaption style="font-size:0.85rem; color:#555; margin-top:0.4rem;">
    Figure 1: Enclosure 1a
  </figcaption>
</figure>

---

**Design Iterations**  

* Iteration 1a-1b: Improved fit for components and manufacturability, but still had tradeoffs (bulk + cable management).

<figure style="width:400px; margin:0 auto; text-align:center;">
  <img src="{{ "/assets/images/virtual-fencing/case-1a.jpeg" | relative_url }}"
       alt="Enclosure 1a"
       style="display:block; width:100%; margin:0 auto;">
  <figcaption style="font-size:0.85rem; color:#555; margin-top:0.4rem;">
    Figure 2: Enclosure 1a
  </figcaption>
</figure>

<figure style="width:400px; margin:0 auto; text-align:center;">
  <img src="{{ "/assets/images/virtual-fencing/case-1b.JPEG" | relative_url }}"
       alt="Enclosure 1b"
       style="display:block; width:100%; margin:0 auto;">
  <figcaption style="font-size:0.85rem; color:#555; margin-top:0.4rem;">
    Figure 3: Enclosure 1b
  </figcaption>
</figure>

* Iteration 2 (best current direction): Designed for lights + most components, manufacturable, slightly larger, with no major listed drawbacks.

<figure style="width:400px; margin:0 auto; text-align:center;">
  <img src="{{ "/assets/images/virtual-fencing/case-2a.jpeg" | relative_url }}"
       alt="Enclosure 2"
       style="display:block; width:100%; margin:0 auto;">
  <figcaption style="font-size:0.85rem; color:#555; margin-top:0.4rem;">
    Figure 4: Enclosure 2
  </figcaption>
</figure>

* Future Iteration 1: Designed to give a larger aurface area incontact with the ear of the cow.

<figure style="width:400px; margin:0 auto; text-align:center;">
  <img src="{{ "/assets/images/virtual-fencing/future-case-3.jpeg" | relative_url }}"
       alt="Future Enclosure 1"
       style="display:block; width:100%; margin:0 auto;">
  <figcaption style="font-size:0.85rem; color:#555; margin-top:0.4rem;">
    Figure 5: Future Enclosure 1
  </figcaption>
</figure>

* Future Iteration 2: Designed to allow more space for electronics and to redistribute weight on ear.

<figure style="width:400px; margin:0 auto; text-align:center;">
  <img src="{{ "/assets/images/virtual-fencing/future-case-4.jpeg" | relative_url }}"
       alt="Future Enclosure 2"
       style="display:block; width:100%; margin:0 auto;">
  <figcaption style="font-size:0.85rem; color:#555; margin-top:0.4rem;">
    Figure 6: Future Enclosure 2
  </figcaption>
</figure>

---

**Electrical Stimuli Prototyping (team workstream summary)**  

To support the deterrence function, we prototyped and simulated high-voltage electric stimuli circuits (transformer-based and boost-converter-based approaches) and validated behavior in lab testing. For example, a boost converter test achieved ~197.4 Vdc output at ~2.34 mA under the stated drive conditions. 

---

**Extra Photos**

<figure style="width:400px; margin:0 auto; text-align:center;">
  <img src="{{ "/assets/images/virtual-fencing/case-1b-to-hand.JPEG" | relative_url }}"
       alt="enclosure 1b to Hand"
       style="display:block; width:100%; margin:0 auto;">
  <figcaption style="font-size:0.85rem; color:#555; margin-top:0.4rem;">
    Figure 7: Encosure 1b to Hand
  </figcaption>
</figure>

<figure style="width:400px; margin:0 auto; text-align:center;">
  <img src="{{ "/assets/images/virtual-fencing/lights-case.JPEG" | relative_url }}"
       alt="Enclosure 2a"
       style="display:block; width:100%; margin:0 auto;">
  <figcaption style="font-size:0.85rem; color:#555; margin-top:0.4rem;">
    Figure 8: More Enclosure 2
  </figcaption>
</figure>

<figure style="width:400px; margin:0 auto; text-align:center;">
  <img src="{{ "/assets/images/virtual-fencing/cow.png" | relative_url }}"
       alt="Its a cow!"
       style="display:block; width:100%; margin:0 auto;">
  <figcaption style="font-size:0.85rem; color:#555; margin-top:0.4rem;">
    Figure 9: Its a cow!
  </figcaption>
</figure>

