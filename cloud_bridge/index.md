## cloud_bridge

A ZMQ-based package that relays ROS2 messages between nodes on different networks. It supports communication with remote robots using a `DDS(LAN) -> WAN -> DDS(LAN)` architecture.

- Repository: [lge-ros2/cloud_bridge](https://github.com/lge-ros2/cloud_bridge)
- Supported ROS2 distributions: Foxy (main), Dashing (separate branch)

### Key Features

- Server-client architecture for cross-network ROS2 communication
- Support for relaying topic / message / TF data
- Configurable QoS
- Docker support

### Getting Started

```bash
rosdep install --from-paths src --ignore-src -r -y
colcon build

# Server
# After configuring config/server.yaml and config/param.yaml
ros2 launch cloud_bridge cloud_bridge_server.launch.py

# Client
# After configuring config/client.yaml and config/param.yaml
ros2 launch cloud_bridge cloud_bridge_client.launch.py
```

The topics/messages/TFs to relay are configured in `config/param.yaml`.

See the [cloud_bridge README](https://github.com/lge-ros2/cloud_bridge#readme) for more details.

[← Back to home](../)
