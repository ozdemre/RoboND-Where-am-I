# RoboND-Where-am-I
This is My Implementation of Udacity Robotics Software Engineer NanoDegree Program Term-2 Where am I Project

# Where Am I?
This project is the localization project of the Udacity Robotics Software Engineer Nanodegree. For this project, Adaptive Monte Carlo Localization (AMCL) algorithm, also known as Particle Filter, applied in ROS to estimate the robot's pose. See the writeup for an extended discussion of the project's theoretical content on localization and parameter tuning.

## Installation & Build
### ROS Melodic
The project was developed on Ubuntu 18.04 LTS with [ROS Melodic](http://wiki.ros.org/melodic), [Gazebo](http://gazebosim.org/) and [catkin](http://wiki.ros.org/catkin) installed. However it should also work with Ubuntu 16.04 and ROS Kinetic.

### Dependencies
The robot relies on the ``amcl``, ``navigation_stack`` and ``move_base`` ROS packages, which should be installed through ``apt-get``.

### Building the Workspace
Use ``catkin`` to build the packages from source. From ``catkin_ws``, run:

``catkin_make; source devel/setup.bash``

to build the workspace packages and add them to the paths of ROS.

### Running the Scripts
Repo contains two different robots. 
For benchmark robot (udacity_bot) run the following commands in seperate terminals.

``roslaunch udacity_bot udacity_world.launch``

``roslaunch udacity_bot amcl.launch``

``rosrun udacity_bot navigation_goal_u``

For personal robot (ozdemre_bot) run the following commands in seperate terminals.

``roslaunch ozdemre_bot udacity_world.launch``

``roslaunch ozdemre_bot amcl.launch``

``rosrun ozdemre_bot navigation_goal``
