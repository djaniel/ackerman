# Ackermann Ignition 

This is a simulation scenario of a car-like vehicle.

[TOC]

## Set up the apptainer image

```
apptainer build --nv --sandbox ignition.sif ignition.def
apptainer run --nv ignition.sif
```

Once inside the container, proceed as usual.

```
ros2 pkg prefix --share stadium
colcon build --symlink-install
source ~/ros2_ws/install/local_setup.bash
```
Launch the simulation

```
ros2 launch stadium stadium_world.launch.py
```

```
ros2 launch sim_wayp_plan_tools gazebo_bridge.launch.py
```

## References
- The story behind the [launch files](https://github.com/gazebosim/ros_gz/tree/humble/ros_gz_sim)
- Link to more [gazebo worlds](https://app.gazebosim.org/dashboard)