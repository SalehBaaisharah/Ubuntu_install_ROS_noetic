# Install ROS on Jetson Nano




# Requirements

* VirtualBox 6.1.36
* Ubuntu 20.04

# Installation 

To install ROS Noetic follow the steps in http://wiki.ros.org/noetic/Installation/Ubuntu

Pick Desktop-Full Install
```sudo apt install ros-noetic-desktop-full```



To install ROS on Jetson Nano

```
$ sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'

```

```
$ sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654

```

```
$ sudo apt update

```

```
$ sudo apt install ros-noetic-desktop

```

```
$ echo "source /opt/ros/melodic/setup.bash" >> ~/.bashrc 
$ source ~/.bashrc
```

```
$ sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential
$ sudo rosdep init 
$ rosdep update
```

```

```




