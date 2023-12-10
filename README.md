## Optitrack ROS2

### Description
This repository is used to integrate the marker data to the ROS2 environment. Some additions on main.cpp file are done to connect it with ROS2. 

### How to use
#### 1. Download the SDK.
Download the [NatNet SDK](https://s3.amazonaws.com/naturalpoint/software/NatNetSDKLinux/ubuntu/NatNet_SDK_4.1_ubuntu.tar) and extract to third_party.
#### 2. Copy NatNet library to file system
```bash
sudo cp libNatNet.so /usr/local/lib/
sudo ldconfig
```
#### 3. Build the project.
```bash
source install/setup.bash
colcon build
```
#### 4. Run the project.
```bash
ros2 run optitrack_core optitrack_core
```

### Credits
This project uses code from [NatNet_SDK_4.1 by NaturalPoint Inc](https://optitrack.com/software/natnet-sdk/) which is licensed under the Apache 2.0 License.

