# StoneFish USV Simulator
![Blueboat Simulator](https://i.imgur.com/hN2tz8w.jpg)

The repository is a mess right now as it includes all my .scn files from testing and every other file in [Vortex Stonefish Simulator](https://github.com/vortexntnu/vortex-stonefish-sim). 
This will be fixed at a later stage.

For the **currently only working version** of the Blueboat simulator, use the file  
`blueboat_demo.scn`.

This scenario loads the `freyboat.scn` drone, which is:

* Heavily based on `freya.scn`
* Updated with different visuals
* Equipped with **two thrusters** (instead of the usual four)
* Includes additional sensors (IMU for both the Blueboat and the payload)
* Includes a **non-tethered payload**

## Thruster Control

To apply thruster force, publish to the topic:

`/freya/thruster_forces`

This topic expects an array where each element corresponds to a thruster:

`[thruster1_force, thruster2_force]`

## View All ROS 2 Topics

To see a full list of available topics, run:

`ros2 topic list`
