## CLOiSim

Unity 기반의 고성능 멀티로봇 시뮬레이터입니다. [SDFormat(SDF)](http://sdformat.org/) 파일을 파싱해 3D 환경과 로봇을 자동으로 구성하고, ROS2와 연동해 시뮬레이션 기반 로봇 개발을 지원합니다.

- Repository: [lge-ros2/CLOiSim](https://github.com/lge-ros2/CLOiSim)
- ROS2 연동 패키지: [lge-ros2/cloisim_ros](https://github.com/lge-ros2/cloisim_ros)
- 지원 ROS2 배포판: Humble, Jazzy (cloisim_ros 통해 연동)

### Key Features

- SDF 파서를 통한 Unity Visual/Collision/Physics 컴포넌트 자동 매핑
- 센서 지원: 2D/3D LiDAR, 컬러/깊이/시맨틱 카메라, IMU, GPS, 소나, IR
- NVIDIA PhysX 기반 물리엔진 (Temporal Gauss Seidel solver)
- 플러그인 아키텍처 (LaserPlugin, CameraPlugin, MicomPlugin 등)
- actor, light, heightmap, road 등 다양한 월드 요소 지원
- 외부 UI 제어를 위한 WebSocket 인터페이스
- 리눅스 headless 모드 지원

### Getting Started

릴리즈 바이너리를 다운로드하거나 소스에서 직접 빌드할 수 있습니다.

```bash
# 환경변수 설정
export CLOISIM_FILES_PATH=/path/to/resources

# 실행
./run.sh cloisim.world
```

소스 빌드 시 Unity Editor 6000.5.0f1 이상이 필요합니다.

자세한 설치 및 사용법은 [CLOiSim README](https://github.com/lge-ros2/CLOiSim#readme)를 참고하세요.

### ROS2 연동

CLOiSim은 [cloisim_ros](https://github.com/lge-ros2/cloisim_ros) 패키지를 통해 ROS2와 연동됩니다.

```bash
git clone https://github.com/lge-ros2/cloisim_ros.git
rosdep install --from-paths src --ignore-src -r -y
colcon build
ros2 launch cloisim_ros_bringup bringup_launch.py
```

[← Back to home](../)
