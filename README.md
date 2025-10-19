# Surge_G13

# Table of Content
- [Goals](#-Goals)

# Goals
Surge: for better surgeries. This is our university software engineering project that attempts to change the medical landscape around the world. The aim is to assist doctors during meticuluous operations for more efficient control and vision, this will be done by using a secure software combined with trained surgeons. This project will bridge the gap between modern technology and accessibility to all hospitals by being compact, accessible, and mobile. The assets of this tool are that it can perform surgeries faster by enhancing accuracy and ensuring cleaner operations, it provides more sterilized enviroment 

# Layout
1. Workspace (surge_ws)
   - The main folder for the project.
   - Contains all packages and build files.

2. Bringup Package
   - Starts everything at once.
   - Has launch files and basic config.

3. Description Package
   - Holds the robot model (URDF), meshes, and RViz settings.

4. Interfaces Package
   - Stores custom message and service definitions.

5. Control Package
   - Runs the main C++ code to control the robot.

6. Localization Package
   - Helps the robot know where it is.

7. Navigation Package
   - Helps the robot plan and follow paths.

8. Common Files in Each Package
   - `package.xml` → package info  
   - `CMakeLists.txt` → how to build  
   - `include/` → headers  
   - `src/` → source code  
   - `launch/` → launch files  
   - `config/` → settings

9. Build Steps
   - `cd surge_ws`
   - `colcon build`
   - `source install/setup.bash`

10. Run the Robot
   - `ros2 launch my_robot_bringup bringup.launch.py`
