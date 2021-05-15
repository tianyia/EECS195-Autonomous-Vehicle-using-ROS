put the nodes in ~/your_workspace/src/your_package/scripts

dependencies of package: 
  geometry_msgs
  nav_msgs
  roscpp
  rospy
  sensor_msgs
  std_msgs

run gazebo3 simulator map and hector slam, then run: rosrun your_package node_name

make sure to set the x_pos, y_pos and z_pos to 0 in turtlebot3 map launch files.

you need to create publisher nodes for PID_controller and RRT_node

for RRT_node, to make sure the whole map is known, you need to manually explore the map first before starting to test it

The data type for /reference_point , /trajectory and /target_pose is std_msgs.msg.Float64MultiArray, /reference_point and /target_pose uses a 4 sized array [x,y,theta,mode]
