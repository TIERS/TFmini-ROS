# TFmini(Plus)-ROS

TFmini(Plus)'s Examples for ROS.

/ Benewake mini infrared range sensor TFmini ROS package
/ Version 1.0


## Package Information

- Package:	tfmini_ros
- Node:		tfmini_ros_node
 
Published Topics:
```
/tfmini_ros_node/range 		(sensor_msgs/Range)
/tfmini_ros_node/status		(std_msgs/String)
```

The topic `/tfmini_ros_node/range` publishes the detection distance. **The max range is 12 meter.** This node won't publish anny message if no object exists within TFmini's measurement range.

The topic `/tfmini_ros_node/status` publishes:
- `ok` if detection within range
- `error` if failed to read data (in which case the node exists) or if there is a data validation error.
- `out` if no object within range

## Quick Start

Launch the node (defualt serial port is `/dev/ttyS5` for UART on the UP2 pin header):
```
roslaunch tfmini_ros tfmini.launch
```
