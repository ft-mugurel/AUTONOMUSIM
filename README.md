# Formula Student Racecar Simulation in Gazebo

This project is a **Gazebo simulation** of a Formula Student racecar, designed to replicate the behavior of an autonomous racing vehicle. The simulation includes a detailed model of the car, its sensors, and the race environment. It is built using **ROS (Robot Operating System)** and integrates various ROS packages for control, perception, and simulation.

## Dependencies

To run the simulation, ensure the following ROS packages are installed:

```bash
sudo apt-get install ros-kinetic-ackermann-msgs \
ros-kinetic-twist-mux \
ros-kinetic-joy \
ros-kinetic-controller-manager \
ros-kinetic-robotnik-msgs \
ros-kinetic-velodyne-simulator \
ros-kinetic-effort-controllers \
ros-kinetic-velocity-controllers \
ros-kinetic-joint-state-controller \
ros-kinetic-gazebo-ros-control \
ros-kinetic-robotnik-msgs
```

# Overview

## The simulation includes:

  - A high-fidelity model of the Formula Student racecar.

  - Integration of LIDAR and other sensors for perception.

  - Realistic physics and control using Gazebo and ROS controllers.

  - A simulated race environment for testing autonomous driving algorithms.

# Usage

  ## Clone the repository.

  - Install the required dependencies listed above.

  - Build the workspace using catkin_make.

  - Launch the simulation with the provided launch file:

    ``` bash
    roslaunch autonomousim_description sim.launch
    ```
## Features

   - Sensor Integration: LIDAR and other sensors are simulated for perception tasks.

   - Control Systems: Ackermann steering and throttle control are implemented for realistic driving behavior.

   - Customizable Environment: Modify the race track or add obstacles for testing.
