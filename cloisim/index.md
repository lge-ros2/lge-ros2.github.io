## CLOiSim

A high-performance, multi-robot simulator built on Unity. It parses [SDFormat (SDF)](http://sdformat.org/) files to automatically construct 3D environments and robots, and integrates with ROS2 for simulation-based robot development.

- Repository: [lge-ros2/CLOiSim](https://github.com/lge-ros2/CLOiSim)
- ROS2 integration package: [lge-ros2/cloisim_ros](https://github.com/lge-ros2/cloisim_ros)
- Supported ROS2 distributions: Humble, Jazzy (via cloisim_ros)

### Key Features

- Automatic mapping of SDF-parsed elements to Unity Visual/Collision/Physics components
- Sensor support: 2D/3D LiDAR, color/depth/semantic camera, IMU, GPS, sonar, IR
- NVIDIA PhysX-based physics engine (Temporal Gauss Seidel solver)
- Plugin architecture (LaserPlugin, CameraPlugin, MicomPlugin, etc.)
- Support for various world elements such as actors, lights, heightmaps, and roads
- WebSocket interface for external UI control
- Headless mode support on Linux

### Getting Started

You can download a release binary or build from source.

```bash
# Set environment variable
export CLOISIM_FILES_PATH=/path/to/resources

# Run
./run.sh cloisim.world
```

Building from source requires Unity Editor 6000.5.0f1 or later.

See the [CLOiSim README](https://github.com/lge-ros2/CLOiSim#readme) for detailed installation and usage instructions.

### ROS2 Integration

CLOiSim integrates with ROS2 through the [cloisim_ros](https://github.com/lge-ros2/cloisim_ros) package.

```bash
git clone https://github.com/lge-ros2/cloisim_ros.git
rosdep install --from-paths src --ignore-src -r -y
colcon build
ros2 launch cloisim_ros_bringup bringup_launch.py
```

[← Back to home](../)
