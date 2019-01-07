### JACKAL_ROBOT_SIMULATION

### Put all folders in the src folder of a catkin workspace, i.e. catkin_ws/src

$ cp JACKAL_ROBOT_SIMULATION/* ~/catkin_ws/src  
$ cd ~/catkin_ws && catkin_make

### Terminal 1
$ source devel/setup.bash  
$ roslaunch jackal_gazebo jackal_world.launch

### Terminal 2
$ source devel/setup.bash  
$ rosrun rviz rviz
