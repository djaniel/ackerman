# Ackermann Ignition 

This a simulation scenario of a car-like vehicle.

## Set up

```
apptainer build --nv ignition.sif ignition.def
apptainer run --nv ignition.sif
```

Launch the robot
```
ign gazebo -v 4 -r ackermann_steering.sdf
```

Launch the Gazebo bridge

```
source ~/ros2_ws/install/local_setup.bash

```
```
ros2 launch sim_wayp_plan_tools gazebo_bridge.launch.py
```
