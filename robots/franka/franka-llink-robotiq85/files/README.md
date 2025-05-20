# Franka Panda, Dynamixel Servo, and Robotiq Gripper for MoveIt


- MoveIt uses URDF and SRDF files for motion planning
- The SRDF and other MoveIt configuration files are generated based on some configuration parameters and the URDF file using MoveIt Setup Assistant
    - This repository (excluding the URDF folder) contains the MoveIt configuration files for the new URDF
    - To edit the configuration, use ``` roslaunch moveit_setup_assistant setup_assistant.launch ```, select "edit configuration", and select this folder

### Instructions
1. Clone the repo in your workspace 
`git clone git@github.com:ac-rad/panda_robotiq_config.git`
2. build, install, and resource the workspace (`catkin build, source devel/setup.bash`)

3. Launch Rviz with the MoveIt plugin:
``` roslaunch panda_robotiq_config demo.launch ```

A modified MoveIt tutorial file for motion planning can be run as an example. The only changes are modifying the link/group names and the box position for the Robotiq gripper instead of the Panda hand.  

Based on: http://docs.ros.org/en/kinetic/api/moveit_tutorials/html/doc/setup_assistant/setup_assistant_tutorial.html
