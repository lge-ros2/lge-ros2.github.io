## cloisim_ros

A device package that connects the [CLOiSim](../cloisim/) simulator with ROS2. It bridges sensor/actuator data from the simulation to ROS2 topics.

- Repository: [lge-ros2/cloisim_ros](https://github.com/lge-ros2/cloisim_ros)
- Supported ROS2 distributions: Jazzy (main), Humble, Foxy, Dashing (per branch)

### Key Features

- Support for camera, LiDAR, IMU, GPS, and contact/range sensors
- Multi-robot / single-robot modes
- Docker container support
- DDS: CycloneDDS recommended, FastRTPS experimentally supported
- colcon-based test suite

### Getting Started

```bash
git clone https://github.com/lge-ros2/cloisim_ros.git
rosdep install --from-paths src --ignore-src -r -y
colcon build

# Multi-robot mode
ros2 launch cloisim_ros_bringup bringup_launch.py

# Single-robot mode
ros2 launch cloisim_ros_bringup bringup_launch.py single_mode:=True
```

See the [cloisim_ros README](https://github.com/lge-ros2/cloisim_ros#readme) for more details.

[← Back to home](../)
