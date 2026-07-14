## Welcome to LGE-ROS2

`lge-ros2` is an open-source project collection heading toward next-generation robotics through a cloud robotics framework connected via 5G. You can browse all repositories on the [GitHub organization](https://github.com/lge-ros2).

### Projects

#### Simulation

**[CLOiSim](cloisim/)** — A high-performance, multi-robot simulator built on Unity. It parses SDFormat (SDF) files to automatically construct 3D environments and robots, and supports a range of sensors (LiDAR, camera, IMU, GPS) along with the NVIDIA PhysX physics engine.
- Repository: [lge-ros2/CLOiSim](https://github.com/lge-ros2/CLOiSim)

**[cloisim_ros](cloisim_ros/)** — A device package that connects the CLOiSim simulator with ROS2. It supports camera, LiDAR, IMU, GPS, and contact/range sensors, along with multi-robot/single-robot modes and Docker execution.
- Repository: [lge-ros2/cloisim_ros](https://github.com/lge-ros2/cloisim_ros)

#### Networking

**[cloud_bridge](cloud_bridge/)** — A ZMQ-based bridge package that relays ROS2 messages (topic/message/TF) between nodes on different networks. It supports remote robot communication with a `DDS(LAN) -> WAN -> DDS(LAN)` architecture.
- Repository: [lge-ros2/cloud_bridge](https://github.com/lge-ros2/cloud_bridge)

### Other repositories

| Repository | Description |
| --- | --- |
| [sample_resources](https://github.com/lge-ros2/sample_resources) | Sample SDF world/model files |
| [navigation2](https://github.com/lge-ros2/navigation2) | ROS2 Navigation Framework and System |
| [ros2_robot_data_collector](https://github.com/lge-ros2/ros2_robot_data_collector) | A node that subscribes to robot topics and records synchronized observation data |
| [sdformat-sharp](https://github.com/lge-ros2/sdformat-sharp) | A C# implementation of SDFormat (Unity package) |
| [rslidar_sdk](https://github.com/lge-ros2/rslidar_sdk) | RoboSense LiDAR SDK (ROS/ROS2) |
| [cloi_common_interfaces](https://github.com/lge-ros2/cloi_common_interfaces) | Common interface (.msg/.srv) definitions |

See the [GitHub organization page](https://github.com/lge-ros2?tab=repositories) for more repositories.

### Support or Contact

For issues or questions, please use GitHub Issues on the relevant repository.
