# slam_map_-navigation

### Launch Simulation World

export TURTLEBOT3_MODEL=burger

roslaunch turtlebot3_gazebo turtlebot3_world.launch

### Run Navigation Node

export TURTLEBOT3_MODEL=burger

roslaunch turtlebot3_navigation turtlebot3_navigation.launch map_file:=$HOME/map.yaml

### Estimate Initial Pose

Click the 2D Pose Estimate button in the RViz menu.

Click on the map where the actual robot is located and drag the large green arrow toward the direction where the robot is facing.

Repeat step 1 and 2 until the LDS sensor data is overlayed on the saved map.

Launch keyboard teleoperation node to precisely locate the robot on the map.

roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch


![photo_2021-07-08_17-17-50](https://user-images.githubusercontent.com/85003576/124937980-8cb98880-e010-11eb-8bac-47db06076b15.jpg)

