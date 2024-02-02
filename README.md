# My simulation environment for the turtlebot3.

Hey there, I developed a simple project (aka rosject) in The Construct Sim.

## How to use
- rosject link: https://app.theconstructsim.com/l/5f5faa8d/

```bash
source ~/ros_ws/install/setup.bash
ros2 launch turtlebot3_gazebo turtlebot3_tc_world_two_robots.launch.py
```

A new window should open with gazebo, wait some seconds until it finishes loading, and search for the turtlebots (sorry for that :c).

## Test on it!
Consider running one (or both) of the following commands.
```bash
ros2 topic pub --once /tb3_0/cmd_vel geometry_msgs/msg/Twist "{linear: {x: 0.2, y: 0.0, z: 0.0}, angular: {x: 0.0, y: 0.0, z: 0.2}}"
ros2 topic pub --once /tb3_1/cmd_vel geometry_msgs/msg/Twist "{linear: {x: 0.2, y: 0.0, z: 0.0}, angular: {x: 0.0, y: 0.0, z: 0.2}}"
```
![Diseño sin título](https://github.com/L4rralde/t3_humble_simulation_pkgs/assets/33332433/e83e6960-6f84-42a4-aa0b-35d39657946a)



Take into account that this is my first rosject, so my instructions might not be the best known.

Best regards,
L4rralde
