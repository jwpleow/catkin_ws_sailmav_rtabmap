# RTAB-Map for SAILMav

## Setup
Build [rtabmap](https://github.com/introlab/rtabmap_ros) from source following the instructions
Get `imu_tools`:
```
sudo apt-get install ros-noetic-imu-tools
```

Place rtabmap_gui.ini in `/home/$USER/.ros/` and fix the first line in the file.   

### IMU Calibration
Perform simple IMU calibration:
```
rosrun imu_calib do_calib
```


## Launch
```
# start camera and imu pub on SailMAV https://github.com/jwpleow/SailMAV_ROS_RPI (use correct branch for IMU)
# start rectifier and depth inference node https://github.com/jwpleow/stereo_libtorch_inference

roslaunch rtabmap_sailmav.launch
```
