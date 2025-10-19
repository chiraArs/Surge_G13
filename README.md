# Surge_G13

# Table of Content
- [Goals](#-goals)

# Goals
Surge: for better surgeries. This is our university software engineering project that attempts to change the medical landscape around the world. The aim is to assist doctors during meticuluous operations for more efficient control and vision, this will be done by using a secure software combined with trained surgeons. This project will bridge the gap between modern technology and accessibility to all hospitals by being compact, accessible, and mobile. The assets of this tool are that it can perform surgeries faster by enhancing accuracy and ensuring cleaner operations, it provides more sterilized enviroment 

# Layout
├── src/                         # All source packages live here
│   ├── my_robot_bringup/        # Launch + configuration package
│   │   ├── launch/
│   │   │   └── bringup.launch.py
│   │   ├── config/
│   │   │   └── robot_params.yaml
│   │   ├── package.xml
│   │   └── CMakeLists.txt
│   │
│   ├── my_robot_description/    # URDF/Xacro, meshes, robot description
│   │   ├── urdf/
│   │   │   └── my_robot.urdf.xacro
│   │   ├── meshes/
│   │   │   ├── base_link.stl
│   │   │   └── arm.stl
│   │   ├── rviz/
│   │   │   └── my_robot_config.rviz
│   │   ├── package.xml
│   │   └── CMakeLists.txt
│   │
│   ├── my_robot_control/        # Control nodes
│   │   ├── src/
│   │   │   ├── controller_node.cpp
│   │   │   └── pid.cpp
│   │   ├── include/my_robot_control/
│   │   │   └── pid.hpp
│   │   ├── launch/
│   │   │   └── control.launch.py
│   │   ├── package.xml
│   │   └── CMakeLists.txt
│   │
│   ├── my_robot_interfaces/     # Custom ROS 2 interfaces
│   │   ├── msg/
│   │   │   └── WheelSpeeds.msg
│   │   ├── srv/
│   │   │   └── SetSpeed.srv
│   │   ├── package.xml
│   │   └── CMakeLists.txt
│   │
│   └── my_robot_navigation/     # Navigation and planning nodes
│       ├── src/
│       │   └── nav_node.py
│       ├── launch/
│       │   └── nav.launch.py
│       ├── config/
│       │   └── nav_params.yaml
│       ├── package.xml
│       └── setup.py
│
├── install/                     # Generated after build
├── build/                       # Build artifacts
├── log/                         # Logs
└── colcon.pkg                   # Optional metadata file
