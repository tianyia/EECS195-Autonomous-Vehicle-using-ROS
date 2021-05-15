put the build_map_automatic node in ~/your_workspace/src/your_package/scripts

dependencies of package: 
  geometry_msgs
  nav_msgs
  roscpp
  rospy
  sensor_msgs
  std_msgs

run gazebo3 simulator map and hector slam, then run: rosrun your_package build_map_automatic

The node should be able to run without problem by the upper instructions
