---
layout: project
title: Shade Splash
description: Cooperative 1D color-matching game
technologies: [Arduino, CAD, Prototyping, Electronics, Physical Computing]
image: /assets/images/shade-splash/holding-controllers.jpeg
---

**Overview**  

Shade Splash is a cooperative 1D color-matching game designed for physical interaction, where two players work together to recreate a target color through coordinated motion and communication. Each player controls a different color, and their combined movements determine the final blended shade displayed in real time. The project explored how physical controllers and embodied interaction can encourage collaboration rather than competition.

<video width="100%" controls>
  <source src="{{ '/assets/images/shade-splash/shade-splash-video.mp4' | relative_url }}" type="video/mp4">
  Your browser does not support the video tag.
</video>

---

**Game Mechanics**  

Players begin in opposite corners of a rectangular play space. A Target Color displayed at the top of the screen indicates the color they must recreate, while a Current Blend at the bottom shows the real-time result of their combined inputs. Each player uses a motion-based controller that acts like a balance wheel: holding the controller parallel to the ground keeps the character stationary, while tilting it left or right moves the character accordingly. Players must coordinate their movements to mix colors accurately. Once they believe the correct shade has been achieved, both players must press their corresponing buttons on their controller to lock down on their desired shade. If successful, the game advances to a new round with a different target color and more shade choices. 

<figure style="width:400px; margin:0 auto; text-align:center;">
  <img src="{{ "/assets/images/shade-splash/game-controls.png" | relative_url }}"
       alt="Game Controls"
       style="display:block; width:100%; margin:0 auto;">
  <figcaption style="font-size:0.85rem; color:#555; margin-top:0.4rem;">
    Figure 1: Game Controls
  </figcaption>
</figure>

---

**Controller Enclosure Design**  

The physical controllers were designed to resemble paint buckets, reinforcing the theme of mixing colors. Multiple iterations of the bucket geometry were developed, starting all the way from a scrappy prototype (Figure 2) to a fully functional 3D printed version. The many iterations of this controller were used to refine ergonomics, confortability, ease of use, and to find the best way to represent a paint bucket while still funcitong as a game controller.

*Paint Bucket Iterations:*

<figure style="width:400px; margin:0 auto; text-align:center;">
  <img src="{{ "/assets/images/shade-splash/design-process.png" | relative_url }}"
       alt="Scrapy Prototypes"
       style="display:block; width:100%; margin:0 auto;">
  <figcaption style="font-size:0.85rem; color:#555; margin-top:0.4rem;">
    Figure 2: Scrapy Prototypes
  </figcaption>
</figure>

<figure style="width:400px; margin:0 auto; text-align:center;">
  <img src="{{ "/assets/images/shade-splash/design-process-2.png" | relative_url }}"
       alt="3D Printed Prototypes"
       style="display:block; width:100%; margin:0 auto;">
  <figcaption style="font-size:0.85rem; color:#555; margin-top:0.4rem;">
    Figure 3: 3D Printed Prototypes
  </figcaption>
</figure>

*Final Design Exploded Views:*

<figure style="width:400px; margin:0 auto; text-align:center;">
  <img src="{{ "/assets/images/shade-splash/exploded-view.png" | relative_url }}"
       alt="Controller Exploded View"
       style="display:block; width:100%; margin:0 auto;">
  <figcaption style="font-size:0.85rem; color:#555; margin-top:0.4rem;">
    Figure 4: Controller Exploded View
  </figcaption>
</figure>

<figure style="width:400px; margin:0 auto; text-align:center;">
  <img src="{{ "/assets/images/shade-splash/exploded-board-view.png" | relative_url }}"
       alt="Protoboard Enclosure Exploded View"
       style="display:block; width:100%; margin:0 auto;">
  <figcaption style="font-size:0.85rem; color:#555; margin-top:0.4rem;">
    Figure 5: Protoboard Enclosure Exploded View
  </figcaption>
</figure>


*Diffusive Layer/LED Layer:*

<figure style="width:400px; margin:0 auto; text-align:center;">
  <img src="{{ "/assets/images/shade-splash/led-layer.png" | relative_url }}"
       alt="LED Layer"
       style="display:block; width:100%; margin:0 auto;">
  <figcaption style="font-size:0.85rem; color:#555; margin-top:0.4rem;">
    Figure 6: Diffusive Layer/Led Layer
  </figcaption>
</figure>

*Fluid:*

<figure style="width:400px; margin:0 auto; text-align:center;">
  <img src="{{ "/assets/images/shade-splash/fluid.png" | relative_url }}"
       alt="Fluid"
       style="display:block; width:100%; margin:0 auto;">
  <figcaption style="font-size:0.85rem; color:#555; margin-top:0.4rem;">
    Figure 7: Fluid
  </figcaption>
</figure>

**Electronic Design**

Each controller housed a 25 count strip of LEDs, a button, and a MPU6050(gyroscope). All wires from each controller housing fed into a second housing enclouser which an Arduino Micro Pro and connected all the electronics on a self-soldered protoboard. The controllers are powered through the type-c port on the Arduino Micro Pro and serves as an output to configure the game on a screen.

*Protoboard Enclosure:*

<figure style="width:400px; margin:0 auto; text-align:center;">
  <img src="{{ "/assets/images/shade-splash/circuit.png" | relative_url }}"
       alt="Circuit Design"
       style="display:block; width:100%; margin:0 right;">
  <figcaption style="font-size:0.85rem; color:#555; margin-top:0.4rem;">
    Figure 8: Circuit Design
  </figcaption>
</figure>

<figure style="width:400px; margin:0 auto; text-align:center;">
  <img src="{{ "/assets/images/shade-splash/real-circuit.png" | relative_url }}"
       alt="Actual Circuit"
       style="display:block; width:100%; margin:0 auto;">
  <figcaption style="font-size:0.85rem; color:#555; margin-top:0.4rem;">
    Figure 9: Actual Circuit
  </figcaption>
</figure>

---

**My Contributions**  

I led the design and fabrication of the physical game controllers, focusing on translating digital game mechanics into intuitive, embodied interaction. Using Fusion 360, I designed and iterated on multiple paint-bucket-inspired enclosures, refining the external form and internal layout to improve ergonomics, balance, and component fit across several versions. I also contributed to rapid prototyping efforts through cardboard mockups and 3D-printed iterations, using each build to inform design revisions related to usability and assembly.

On the electronics side, I helped integrate and test the controller hardware, including the Arduino Pro Micro, MPU6050 gyroscope, LED strips, push buttons, and custom PCB. I supported wiring layout and enclosure integration, working through multiple internal configurations to reduce complexity and improve reliability. To enhance the tactile realism of the controllers, I participated in testing different “fluid” materials—including rice, water, ball bearings, and wrapped ball bearings—to emulate the feeling of pouring paint while maintaining durability and consistency during gameplay.

---

**Renderings**

<figure style="width:400px; margin:0 auto; text-align:center;">
  <img src="{{ "/assets/images/shade-splash/rendering-1.png" | relative_url }}"
       alt="Rendering 1"
       style="display:block; width:100%; margin:0 auto;">
  <figcaption style="font-size:0.85rem; color:#555; margin-top:0.4rem;">
    Figure 10: Rendering 1
  </figcaption>
</figure>

<figure style="width:400px; margin:0 auto; text-align:center;">
  <img src="{{ "/assets/images/shade-splash/rendering-2.png" | relative_url }}"
       alt="Rendering 2"
       style="display:block; width:100%; margin:0 auto;">
  <figcaption style="font-size:0.85rem; color:#555; margin-top:0.4rem;">
    Figure 11: Rendering 2
  </figcaption>
</figure>

<figure style="width:400px; margin:0 auto; text-align:center;">
  <img src="{{ "/assets/images/shade-splash/rendering-3.png" | relative_url }}"
       alt="Rendering 3"
       style="display:block; width:100%; margin:0 auto;">
  <figcaption style="font-size:0.85rem; color:#555; margin-top:0.4rem;">
    Figure 12: Rendering 3
  </figcaption>
</figure>

**More Pictures**
<figure style="width:400px; margin:0 auto; text-align:center;">
  <img src="{{ "/assets/images/shade-splash/button.JPEG" | relative_url }}"
       alt="Button Close-Up"
       style="display:block; width:100%; margin:0 auto;">
  <figcaption style="font-size:0.85rem; color:#555; margin-top:0.4rem;">
    Figure 13: Button Close-Up
  </figcaption>
</figure>

<figure style="width:400px; margin:0 auto; text-align:center;">
  <img src="{{ "/assets/images/shade-splash/front-view.JPEG" | relative_url }}"
       alt="Front View"
       style="display:block; width:100%; margin:0 auto;">
  <figcaption style="font-size:0.85rem; color:#555; margin-top:0.4rem;">
    Figure 14: Front View
  </figcaption>
</figure>

<figure style="width:400px; margin:0 auto; text-align:center;">
  <img src="{{ "/assets/images/shade-splash/holding-controllers.jpeg" | relative_url }}"
       alt="Controllers in Hand"
       style="display:block; width:100%; margin:0 auto;">
  <figcaption style="font-size:0.85rem; color:#555; margin-top:0.4rem;">
    Figure 15: Controllers in Hand
  </figcaption>
</figure>

<figure style="width:400px; margin:0 auto; text-align:center;">
  <img src="{{ "/assets/images/shade-splash/holding-with-screen.jpg" | relative_url }}"
       alt="Controllers in Hand with Screen"
       style="display:block; width:100%; margin:0 auto;">
  <figcaption style="font-size:0.85rem; color:#555; margin-top:0.4rem;">
    Figure 16: Controllers in Hand with Screen
  </figcaption>
</figure>

<figure style="width:400px; margin:0 auto; text-align:center;">
  <img src="{{ "/assets/images/shade-splash/pouring-look.jpeg" | relative_url }}"
       alt="Pouring Look"
       style="display:block; width:100%; margin:0 auto;">
  <figcaption style="font-size:0.85rem; color:#555; margin-top:0.4rem;">
    Figure 17: Pouring Look
  </figcaption>
</figure>

<figure style="width:400px; margin:0 auto; text-align:center;">
  <img src="{{ "/assets/images/shade-splash/spout.png" | relative_url }}"
       alt="Spout"
       style="display:block; width:100%; margin:0 auto;">
  <figcaption style="font-size:0.85rem; color:#555; margin-top:0.4rem;">
    Figure 18: Spout
  </figcaption>
</figure>

<figure style="width:400px; margin:0 auto; text-align:center;">
  <img src="{{ "/assets/images/shade-splash/top-slant-view.JPEG" | relative_url }}"
       alt="Final View"
       style="display:block; width:100%; margin:0 auto;">
  <figcaption style="font-size:0.85rem; color:#555; margin-top:0.4rem;">
    Figure 19: Final View
  </figcaption>
</figure>
