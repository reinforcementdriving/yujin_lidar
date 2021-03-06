# Yujin LiDAR
Official Website: http://lidar.yujinrobot.com/

## About Yujin LiDAR

YRL series LiDAR is designed to detect objects, measure distances from surroundings and collect data as point clouds. Yujin LiDAR is an optimized solution for indoor mapping, navigation, localization and other applications in a variety of industries including robotics, safety and security.
## Videos of 3D SLAM and Obstacle Detection
![](slam_F1.gif)
![](slam_F1_2.gif)
![](od_1.gif)
![](od_2.gif)
![](od_3.gif)

## ROS Package Maintenance

- ROS Version: Melodic
- Maintainer Status: Developed
- Author: Ju Young Kim
- License: BSD

![](github_rosdriver.gif)

## Supported Hardware

- YRL2-05 (2D, 5m)
- YRL2-15 (2D, 15m)
- YRL2-25 (2D, 25m)
- YRL3-05 (3D, 5m)
- YRL3-15 (3D, 15m)
- YRL3-25 (3D, 25m)

## ROS Package Installation

```bash
source /opt/ros/melodic/setup.bash
mkdir -p ~/catkin_ws/src/
cd ~/catkin_ws/src/
git clone https://
cd ..
catkin_make
source ~/catkin_ws/devel/setup.bash
rospack profile
```

## ROS API
- Package Name: yujin_yrl3_package
- Node Name: yrl3_pub
- Publisher Name : yrl3_pub
- Topic Name : yrl3_cloud
### Parameters
YRL ROS driver imports YRL Linux driver. To get and set parameters of YRL ROS driver, please use APIs explained in the manual.

## QUICK START
```bash
rosrun yujin_yrl3_package yrl3_pub
rostopic echo /yrl3_pub/yrl3_cloud
rosrun rviz rviz
```
## Additional Software
### Viewer
- Ubuntu 18.04 is required.
#### For Linux: Dependency Installation
```bash
sudo apt-get install qt5-default
```
#### For Linux: Quick Start For Viewer
```bash
cd dir_of_Yujin_Lidar_Viewer
sudo chmod 777 Yujin_Lidar_Viewer
./Yujin_Lidar_Viewer
```

- IP Address Chaning Tool
## Documents
- Catalog
- User manual
- Communication Protocol Specification
- 2D/3D CAD

------------------------------------------------------------------------
![lidar](https://upload.wikimedia.org/wikipedia/commons/2/22/Yujin_lidar.jpg "Yujin Lidar")
![Yujin Logo](https://upload.wikimedia.org/wikipedia/commons/0/0f/Yujinrobot_logo.png "Yujin Logo")
