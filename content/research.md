---
title: "Research"
date: 2020-12-28T11:24:32+05:30
draft: false
description: Past and current projects.
---

<h3>Damaged fault zones and seismic cycles</h3> 

I am currently working on understanding the effect of low velocity zones surrounding an active fault on long term fault slip. Such a setting is common in mature faults like San Andreas, California, and Northern Anatolian, Turkey.  We use mechanical models with prescribed stresses and friction to solve the elastodynamic equation of motion. The earthquake rupture sequences in the cycle happen spontaneously as a result of self-organized stresses, and is not defined by the user. Our models can capture all the stages of the seismic cycle including earthquake nucleation, dynamic rupture propagation, and postseismic and interseismic deformation. My research involves studying how these low velocity fault damage zones affect the earthquake sequences over long term and how these fault damage zones evolve through these different stages of the seismic cycle. I am also involved in developing a Julia code for these simulations to solve the equations efficiently and get increased performance. Code: [https://github.com/thehalfspace/Spear](https://github.com/thehalfspace/Spear)

<h3>Intraslab stresses in Sumatra-Andaman subduction zone and Burma plate</h3>

Earthquakes can tell us a lot about the tectonics of a region. Using global moment tensor data for earthquakes, we can obtain the earthquake focal mechanisms and therefore the net slip direction along various fault planes. Similar to what is described below, we can invert slip directions from multiple faults to get the regional stress state. In our Sumatra-Andaman subduction zone setting, we studied the variation in the stresses of the different parts of subducting and overriding
slabs. Some [codes and results](https://github.com/thehalfspace/GMT_Plots).

<h3>New methods for paleostress analysis using fault-slip data</h3>

Structural geologists often aim to quantify regional paleo-stresses based on field observations, usually in the form of slip lineations on a fault. The orientation of these lineations is generally coherent with the direction of maximum shear stress acting on that fault plane. Using multiple observations, we can invert for the stresses. This inversion is highly nonlinear, and requires sophisticated techniques to get a best estimate. To make matters worse, the field observations contain data from multiple stress states that acted in different times in the geological past. We developed an [efficient numerical inversion technique](https://github.com/thehalfspace/stress-inversion) using genetic algorithms to cluster and invert for the multiple stress states without apriori knowledge about the number of stress states.
