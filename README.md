CIS565: Project 3: CUDA Simulation and GLSL Visualization
===
Fall 2013
---
Due Sunday, 10/20/2013 by 11:59:59 pm
---

PART 1: CUDA NBody Simulation
===
This is the basic tutorial part. I'd done with this part, as well as the shared memory force calculation. You can find the performance evaluation below for this shared memory part.


PART 2: Your CUDA Simulation
===

---
VIDEO LINK
---
http://youtu.be/ffbJMcmOPHc

Do feel free to watch my demo on the above link.

---
INTRODUCTION
---
I had implemented 2 simulations for this project: cloth simulation and flocking behavior simulation. 

In the cloth simulation, I simulate a cloth which is modeled as a 200*200 mass-spring system. Each knot of the cloth 
have 12 springs: 4 structure springs, 4 shear springs and 4 bend springs. Each spring is calculated upon its original length as the value when it is set up. Coeff values for all three kinds of springs can be modified 
easily in the kernel.h. I do not implement the collision detection part because of the the time is limited. Instead, I add a wind-force-field in this simulation so that it can wave as the wind blows.

In the flocking behaviors simulation, I used 12,000 agents in the demo video. The flocking behavior have 4 component behaviours: cohesion, which is used to group them together; separation, which guarantee the minimum 
distance between the agents; alignment, make sure that the neighbour agents shall go to the same direction; and wander, which add some noise to the individuals. Coeff values are also listed in the kernel.h. 

On the interaction side, I add the mouse interaction which enable the user to manipulate the camera with zoom in/out, move left/right, rotate left/ right. On the glsl side, I change the code so that it will render as pyramids
 for each point, with different colors.
 
 So all above are generally the work I'd done with. And I'll explain them in detail below.

---
CLOTH SIMULATION
---


///NEED TO BE IMPLEMENTED

---
FLOCKING SIMULATION
---
///NEED TO BE IMPLEMENTED

---
PERFORMANCE EVALUATION
---
///NEED TO BE IMPLEMENTED

---
SCREENSHOTS
---
///LATER


---
THIRD PARTY CODE
---
None except for the basecode. Everything else are scratched up, including the mouse interaction

