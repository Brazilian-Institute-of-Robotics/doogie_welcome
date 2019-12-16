# Doogie Welcome

## Overview
A basic package for first user interaction with the Doogie Mouse and ROS

**Keywords:** Doogie Mouse, Micromouse, ROS

### License
The source code is released under a [Apache License 2.0](https://github.com/Brazilian-Institute-of-Robotics/jiro_efuse_driver/blob/master/LICENSE).

**Author:** Mateus Menezes
**Affiliation:** Brazilian Institute of Robotics - BIR
**Maintainer:** Mateus Menezes, mateusmenezes95@gmail.com
**Maintainer:** Caio Amaral, caioaamaral@gmail.com

The Doogie Welcome package has been tested under ROS Kinetic and Ubuntu 16.04 LTS and Raspbian Jessie Desktop.

## Installation
> **Note:** Skip this step if your workspace has already created!

Create a new workspace where the Doogie Mouse packages will be installed and build it:
```sh
$ mkdir -p ~/doogie_ws/src
$ cd ~/doogie_ws
$ catkin_make
```

Clone the `doogie_welcome` package into the workspace:
```sh
$ cd ~/doogie_ws/src
$ git clone https://github.com/doogie-mouse/doogie_welcome.git
```

### Building from source
After instalation, run the following commands to build it: 
```sh
$ cd ~/doogie_ws
$ catkin_make
```

## Usage

Run the main node with
```sh
$ roslaunch doogie_welcome doogie_welcome.launch
```

## Launch file

* **[doogie_welcome.launch](launch/doogie_welcome.launch):** Launch the node of the ROS Driver

## Nodes
TODO

#### Published Topics

* **`/cpp_chatter`** ([std_msgs/String])
	TODO.

* **`/python_chatter`** ([std_msgs/String])
	TODO.

#### Subscribed Topics

* **`/cpp_chatter`** ([std_msgs/String])
	TODO.

* **`/python_chatter`** ([std_msgs/String])
	TODO.
  
## Bugs & Feature Requests

Please report bugs and request features using the [Issue Tracker](https://github.com/doogie-mouse/doogie_welcome/issues).


[std_msgs/String]: http://docs.ros.org/api/std_msgs/html/msg/String.html
