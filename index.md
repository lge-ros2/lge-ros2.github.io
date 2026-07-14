## Welcome to LGE-ROS2

`lge-ros2`는 클라우드 로보틱스(Cloud Robotics) 프레임워크와 5G 연결을 기반으로 차세대 로보틱스를 지향하는 오픈소스 프로젝트 모음입니다. 전체 저장소는 [GitHub organization](https://github.com/lge-ros2)에서 확인할 수 있습니다.

### Projects

#### [CLOiSim](cloisim/)
Unity 기반의 고성능 멀티로봇 시뮬레이터입니다. SDFormat(SDF) 파일을 파싱해 3D 환경과 로봇을 자동으로 구성하며, LiDAR/카메라/IMU/GPS 등 다양한 센서와 NVIDIA PhysX 물리엔진을 지원합니다.
- Repository: [lge-ros2/CLOiSim](https://github.com/lge-ros2/CLOiSim)

#### [cloisim_ros](cloisim_ros/)
CLOiSim 시뮬레이터와 ROS2를 연결해주는 디바이스 패키지입니다. 카메라, LiDAR, IMU, GPS, contact/range 센서를 지원하며 멀티로봇/싱글로봇 모드와 Docker 실행을 지원합니다.
- Repository: [lge-ros2/cloisim_ros](https://github.com/lge-ros2/cloisim_ros)

#### [cloud_bridge](cloud_bridge/)
ZMQ 기반으로 서로 다른 네트워크에 있는 ROS2 노드 간 메시지(topic/message/TF)를 중계하는 브릿지 패키지입니다. `DDS(LAN) -> WAN -> DDS(LAN)` 구조로 원격지 로봇과의 통신을 지원합니다.
- Repository: [lge-ros2/cloud_bridge](https://github.com/lge-ros2/cloud_bridge)

### Other repositories

| Repository | 설명 |
| --- | --- |
| [sample_resources](https://github.com/lge-ros2/sample_resources) | SDF 샘플 world/model 파일 모음 |
| [navigation2](https://github.com/lge-ros2/navigation2) | ROS2 Navigation Framework and System |
| [ros2_robot_data_collector](https://github.com/lge-ros2/ros2_robot_data_collector) | 로봇 토픽을 구독해 동기화된 관측 데이터를 기록하는 노드 |
| [sdformat-sharp](https://github.com/lge-ros2/sdformat-sharp) | SDFormat의 C# 구현 (Unity 패키지) |
| [rslidar_sdk](https://github.com/lge-ros2/rslidar_sdk) | RoboSense LiDAR SDK (ROS/ROS2) |
| [cloi_common_interfaces](https://github.com/lge-ros2/cloi_common_interfaces) | 공용 인터페이스(.msg/.srv) 모음 |

더 많은 저장소는 [GitHub organization 페이지](https://github.com/lge-ros2?tab=repositories)에서 확인하세요.

### Support or Contact

이슈나 문의사항은 각 저장소의 GitHub Issues를 이용해 주세요.
