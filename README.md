# Install ROS on Jetson Nano




# Requirements

* VirtualBox 6.1.36
* Ubuntu 20.04

# Installation 

To install ROS Noetic follow the steps in http://wiki.ros.org/noetic/Installation/Ubuntu

Pick Desktop Install
```sudo apt install ros-noetic-desktop```



To install ROS on Jetson Nano

Set up the Jetson Nano
```
$ sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu 
$(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'

```
Add a new apt key
```
$ sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654

```
Update the Debian packages index
```
$ sudo apt update

```
Update your .bashrc script:

```
$ echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc 
$ source ~/.bashrc
```
Install and initialize rosdep. rosdep 
```
$ sudo apt install python3-rosdep python3-rosinstall python3-rosinstall-generator python3-wstool build-essential
$ sudo rosdep init 
$ rosdep update
```





