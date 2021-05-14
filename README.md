# RTAB-Map for SAILMav

## Setup
Build rtabmap and imu_calib

```
sudo apt-get install ros-noetic-imu-tools
```

### Stuff
Place rtabmap_gui.ini in `/home/$USER/.ros/` and fix the first line in the file.   

### IMU Calibration
```
rosrun imu_calib do_calib
```


