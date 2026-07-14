## cloisim_ros

[CLOiSim](../cloisim/) 시뮬레이터와 ROS2를 연결해주는 디바이스 패키지입니다. 시뮬레이션 내 센서/액추에이터 데이터를 ROS2 토픽으로 브릿징합니다.

- Repository: [lge-ros2/cloisim_ros](https://github.com/lge-ros2/cloisim_ros)
- 지원 ROS2 배포판: Jazzy(메인), Humble, Foxy, Dashing (브랜치별)

### Key Features

- 카메라, LiDAR, IMU, GPS, contact/range 센서 지원
- 멀티로봇 / 싱글로봇 모드
- Docker 컨테이너 지원
- DDS: CycloneDDS 권장, FastRTPS 실험적 지원
- colcon 기반 테스트 스위트

### Getting Started

```bash
git clone https://github.com/lge-ros2/cloisim_ros.git
rosdep install --from-paths src --ignore-src -r -y
colcon build

# 멀티로봇 모드
ros2 launch cloisim_ros_bringup bringup_launch.py

# 싱글로봇 모드
ros2 launch cloisim_ros_bringup bringup_launch.py single_mode:=True
```

자세한 내용은 [cloisim_ros README](https://github.com/lge-ros2/cloisim_ros#readme)를 참고하세요.

[← Back to home](../)
