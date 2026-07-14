## cloud_bridge

ZMQ 기반으로 서로 다른 네트워크에 있는 ROS2 노드 간 메시지를 중계하는 패키지입니다. `DDS(LAN) -> WAN -> DDS(LAN)` 구조로 원격지 로봇과의 통신을 지원합니다.

- Repository: [lge-ros2/cloud_bridge](https://github.com/lge-ros2/cloud_bridge)
- 지원 ROS2 배포판: Foxy(메인), Dashing(별도 브랜치)

### Key Features

- 서버-클라이언트 구조의 네트워크 간 ROS2 통신
- topic / message / TF 데이터 중계 지원
- QoS 설정 가능
- Docker 지원

### Getting Started

```bash
rosdep install --from-paths src --ignore-src -r -y
colcon build

# 서버
# config/server.yaml, config/param.yaml 설정 후
ros2 launch cloud_bridge cloud_bridge_server.launch.py

# 클라이언트
# config/client.yaml, config/param.yaml 설정 후
ros2 launch cloud_bridge cloud_bridge_client.launch.py
```

`config/param.yaml`에서 중계할 topic/message/TF를 설정합니다.

자세한 내용은 [cloud_bridge README](https://github.com/lge-ros2/cloud_bridge#readme)를 참고하세요.

[← Back to home](../)
