---
layout: project
title: Virtual Fencing (Low-Cost Cow Ear Tag)
description: GPS-based virtual boundary system + iterative ear-tag CAD + electric stimuli prototyping
technologies: [Fusion360, BantamTools, ANSYS]
image: /assets/images/virtual-fencing.png
---

*Overview*  
Virtual fencing is a livestock management approach that uses GPS tracking and stimuli (sound + electric shock) to keep animals within a farmer-defined virtual boundary. Instead of physically moving fences, farmers can set GPS coordinates and track animals in real time, with collars (or tags) triggering stimuli as animals approach the boundary. :contentReference[oaicite:1]{index=1}

*Problem + Motivation*  
Traditional fencing takes time and labor to move and maintain, but current virtual fencing systems are expensive and often rely on bulky, heavy collars that can snag on objects. :contentReference[oaicite:2]{index=2}

*Project Goal*  
Our team was tasked with designing an affordable, low-cost **cow ear tag** alternative to reduce size compared to collars and make virtual fencing more accessible (especially for low and middle income countries). The goal was to monitor cow movement/behavior using sensor data (GPS + accelerometer) and deter boundary crossing using **sound, lights, and electric shock**. :contentReference[oaicite:3]{index=3}

*Customer Discovery (what we learned from farmers / stakeholders)*  
Key concerns that came up were cost, communication/reliability (ex: WiFi issues), and overall trust in the system. We also heard that farmers need flexible fencing sizes across seasons (bigger in summer, smaller in winter). Traditional/electric fencing has its own issues like maintaining charge, longevity, and physical upkeep (wires, branches breaking lines). :contentReference[oaicite:4]{index=4}  
When asked what it would take to invest in a new system, the biggest themes were being forced by circumstances and the need for strong cost + reliability. :contentReference[oaicite:5]{index=5}

*My Contribution (Jamison — CAD + Iteration)*  
I led the mechanical packaging iterations for the ear tag enclosure, focused on reducing bulk and improving manufacturability while still fitting the required components.

*Design Iterations*  
* Iteration 1–2: Easy to take apart, but too bulky and not manufacturable. :contentReference[oaicite:6]{index=6}  
* Iteration 3.1–3.2: Improved fit for components and manufacturability, but still had tradeoffs (bulk + cable management). :contentReference[oaicite:7]{index=7}  
* Iteration 4 (best current direction): Designed for lights + most components, manufacturable, slightly larger, with no major listed drawbacks. :contentReference[oaicite:8]{index=8}

*Electrical Stimuli Prototyping (team workstream summary)*  
To support the deterrence function, we prototyped and simulated high-voltage electric stimuli circuits (transformer-based and boost-converter-based approaches) and validated behavior in lab testing. For example, a boost converter test achieved ~197.4 Vdc output at ~2.34 mA under the stated drive conditions. :contentReference[oaicite:9]{index=9}

*Next Steps*  
Next steps include determining capacitor charge/discharge timing to reliably generate the spark, integrating the circuit with the rest of the system using a 3.7V LiPo battery, and packaging everything into the ear-tag casing. :contentReference[oaicite:10]{index=10}

