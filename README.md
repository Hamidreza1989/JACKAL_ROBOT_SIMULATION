### JACKAL_ROBOT_SIMULATION

### Put all folders in the src folder of a catkin workspace, i.e. catkin_ws/src

$ ln -sf JACKAL_ROBOT_SIMULATION ~/catkin_ws/src  
$ cd ~/catkin_ws && catkin_make

### Terminal 1
$ source devel/setup.bash  
$ roslaunch jackal_gazebo jackal_world.launch

### Terminal 2
$ source devel/setup.bash  
$ rosrun rviz rviz



### JACKAL_NAV_EXAMPLE with PointCloud2 converted to LaserScan
### FIXME! The converted LaserScan cannot see some very close wall in some angles

$ git checkout Neil_local
$ git pull
$ cd ~/catkin_ws && catkin_make 


### Terminal 1
$ source devel/setup.bash  
$ roslaunch jackal_gazebo jackal_world.launch

### Terminal 2
$ source devel/setup.bash  
$ roslaunch jackal_navigation odom_navigation_demo.launch


### Terminal 3
$ source devel/setup.bash  
$ roslaunch jackal_viz view_robot.launch config:=navigation

