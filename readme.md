# HRI hand control

## Overview

This is a ROS package developed for check up the [Realsense camera](http://wiki.ros.org/realsense2_camera) with [AR marker](http://wiki.ros.org/ar_track_alvar).  
The packages have been tested under ROS Kinetic, Ubuntu 16.04, D435i.

**Author: [Hyeonjun Park](https://www.linkedin.com/in/hyeonjun-park-41bb59125), koreaphj91@gmail.com**  
**Affiliation: [Human-Robot Interaction LAB](https://khu-hri.weebly.com), Kyung Hee Unviersity, South Korea**



## Installation
- Before do this, please backup important files.

### Dependencies

This software is built on the Robotic Operating System ([ROS](http://wiki.ros.org/ROS/Installation)).  
One line install: https://cafe.naver.com/openrt/14575 
```
for Desktop

wget https://raw.githubusercontent.com/ROBOTIS-GIT/robotis_tools/master/install_ros_kinetic.sh && chmod 755 ./install_ros_kinetic.sh && bash ./install_ros_kinetic.sh
```

- Realsense ROS ([ref. link](http://emanual.robotis.com/docs/en/platform/openmanipulator_x/ros_applications/#ros-applications))
```
$ sudo apt-key adv --keyserver keys.gnupg.net --recv-key C8B3A55A6F3EFCDE || sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-key C8B3A55A6F3EFCDE
$ sudo add-apt-repository "deb http://realsense-hw-public.s3.amazonaws.com/Debian/apt-repo xenial main" -u
$ sudo apt-get install librealsense2-dev librealsense2-utils ros-kinetic-rgbd-launch

$ cd ~/catkin_ws/src
$ git clone https://github.com/intel-ros/realsense.git
$ cd ~/catkin_ws && catkin_make
```

- ar_track_alvar
```
$ sudo apt-get install ros-kinetic-ar-track-alvar
```


## How to start?

```
$ cd ~/catkin_ws/src && git clone https://github.com/MrLacquer/realsense-ros-armarker.git
$ cd ~/catkin_ws && catkin_make
$ rospack profile && rosstack profile

$ roslaunch realsense-ros-ar-marker realsense_ros_ar_marker_rviz.launch
```


## Demo


