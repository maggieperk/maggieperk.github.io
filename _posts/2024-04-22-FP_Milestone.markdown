---
layout: post
title:  "Final Project: Mid Progress Milestone"
date:   2024-04-22 10:30:54 +0100
categories: comp_fabrication
---
# Elevator Pitch
The goal of my project is to allow someone to laser cut scrap wood to make a custom (parameterized) planter box.  I will create a parameterizable Grasshopper template that will take the desired planter dimensions as input along with the dimensions of the materials available.  Then the file will output a template that can be used to cut down the wood appropriately into 5 pieces that will fit together for a planter.

# Walk Through
The following diagram is a 2D representation of the planter dimensions to better understand the parameters concerned here.
![Planter Layout Diagram](../assets/images/PlanterLayout_MidMilestone.png)
Ideally, someone is able to use my project by going through the following steps:
1. Download the Grasshopper file
2. Adjust the appropriate planter box parameters for their needs
3. Output a file that can be used as input to a laser cutter
4. Cut their materials to the appropriate dimensions
5. Assemble the 5 pieces together with relative ease (due to the joint configuration)
The initial Grasshopper configuration can be seen below with adjustable parameters - right now this does not have the ability to produce the joints, it is representing the output as a set of boxes and needs to look at individual sides.
![Planter Layout Grasshopper](../assets/images/ParamPlanterGH_Initial.png)
