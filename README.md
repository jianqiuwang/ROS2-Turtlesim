---

# **Turtlesim Catch-All Project**

A ROS2-based project utilizing Turtlesim, where the goal is to control a turtle to catch other turtles spawned at random positions.

---

## **Overview**

This project demonstrates basic ROS2 concepts like publishers, subscribers, and services. The main turtle moves around the Turtlesim simulator to "catch" other turtles, which are dynamically spawned at random locations.

---

## **Setup Instructions**

1. Clone this repository:
   ```bash
   cd ~/ros2_ws/src
   git clone git@github.com:jianqiuwang/ROS2-Turtlesim.git
   ```

2. Build the workspace:
   ```bash
   cd ~/ros2_ws
   colcon build
   ```

3. Source the workspace:
   ```bash
   source install/setup.bash
   ```

---

## **Usage**

1. Launch the simulation:
   ```bash
   ros2 launch my_robot_bringup turtlesim_catch_them_all.launch.py
   ```

2. Use the main turtle (`turtle1`) to "catch" other turtles.

3. Additional turtles spawn randomly and are removed upon being caught.

---

## **Code Structure**

- **`my_robot_interfaces/`**: Contains custom messages for turtle tracking.
- **`turtlesim_catch_them_all/`**: Implements the spawning and catching logic.
- **`my_robot_bringup/`**: Contains launch files to start the simulation.

---
