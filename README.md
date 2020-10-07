# TFmini(Plus)-ROS
TFmini(Plus)'s Examples for ROS.  

/**************************************************************************************************************************************
/* Benewake mini infrared range sensor TFmini ROS package
/* Version 1.0
/**************************************************************************************************************************************

## Package Information

- Package:	tfmini_ros
- Node:		tfmini_ros_node
 
Published Topics:
```
/tfmini_ros_node/TFmini (sensor_msgs/Range)
```
The distance of object detected. 
Note: This node won't publish topic if no object exists within TFmini's measurement range.


## Quick Start

Launch the node (defualt serial port is `/dev/ttyS5` for UART on the UP2 pin header):
```
roslaunch tfmini_ros tfmini.launch
```
