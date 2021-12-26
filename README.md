## config/aubo_i3.srdf
SRDF는 로봇에 대한 의미론적 정보의 표현입니다.이 형식은 URDF 파일에 없는 로봇에 대한 정보를 나타내기 위한 것이지만 다양한 애플리케이션에 유용합니다.의도는 의미론적 측면이 있는 정보를 포함하는 것입니다.
## config/ompl_planning.yaml
OMPL(Open Motion Planning Library) 플래닝 플러그인을 구성합니다.
SRDF에 정의된 모든 계획 그룹에 대해 여러 계획 구성이 지정됩니다(planner_configs 아래).
또한 충돌 확인 해결과 같이 특정 그룹에 대해 계획할 상태 공간에 대한 기본 설정을 지정할 수 있습니다.
그룹에 대해 지정된 각 계획 구성은 planner_configs 태그 아래에 정의되어야 합니다.
플래너 구성을 정의하는 동안 유일한 필수 매개변수는 사용할 모션 플래너의 이름인 '유형'입니다.
다른 계획자별 매개변수는 정의할 수 있지만 선택 사항입니다.

## config/chomp_planning.yaml
CHOMP 플래너에 사용할 chomp 계획 플러그인 매개변수를 지정합니다.

## config/kinematics.yaml
SRDF의 각 계획 그룹에 사용할 운동학 솔버 플러그인과 운동학 솔버 검색 해상도를 지정합니다.

## config/joint_limits.yaml
URDF에 포함되지 않은 계획 그룹에 나타나는 관절에 대한 추가 정보가 포함되어 있을 뿐만 아니라 URDF에 포함된 것보다 속도 및 가속도에 대한 최대 및 최소 제한을 설정할 수 있습니다.
이 정보는 궤적 필터링 시스템에서 로봇 컨트롤러에 전달되기 전에 궤적에 대한 적절한 속도와 타이밍을 할당하는 데 사용됩니다.

## config/cartesian_limits.yaml
작업 공간 계획을 위한 데카르트 속도.
속도는 개별 계획 요청의 속도 배율로 조정된 데카르트 계획 요청의 최대 속도로 pilz industrail 모션 플래너에서 사용됩니다.

## config/fake_controllers.yaml
정의된 그룹에 해당하는 컨트롤러에 대한 더미 구성을 생성합니다.
이것은 주로 테스트에 유용합니다.

## config/simple_moveit_controllers.yaml
SimpleMoveitControllerManager에 대한 컨트롤러 구성을 생성합니다.

## config/gazebo_controllers.yaml
Gazebo 컨트롤러의 구성.

## config/ros_controllers.yaml
ros_control에 대한 컨트롤러 구성을 생성합니다.

## config/sensors_3d.yaml
Creates configurations 3d sensors.

## launch/move_group.launch








