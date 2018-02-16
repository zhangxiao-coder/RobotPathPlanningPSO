
# RobotPathPlanningPSO

## Mobile Robot Path Planning Using Particle Swarm Optimization

Evan Krell & Arun Prassanth R.B.

This project explores using [particle swarm optimization (PSO)](https://en.wikipedia.org/wiki/Particle_swarm_optimization) for mobile robot path planning. 
In this system, a simulated [Turtlebot](http://www.turtlebot.com/) is able to generate a map of the environment which it
can then use to generate a path from its current position to a user-specified target position. A very high-level overview of the system flow is summarized in the 
System Flow diagram, below. 

![alt text][system_flow]

[system_flow]: doc/img/system_flow.png "System Flow"

The [Gazebo simulator](http://gazebosim.org/) is used for the Turtlebot and its environment. 
A virtual machine with the environment used is available [here](https://www.mathworks.com/supportfiles/robotics/ros/virtual_machines/v3/installation_instructions.htm).
The Turtlebot is controlled through a MATLAB script on a Windows computer. Communication is handled by [ROS](http://www.ros.org/), 
which is supported by MATLAB's [Robotics System Toolbox](https://www.mathworks.com/products/robotics.html). 
Path planning is done on a separate Linux server. The MATLAB script coordinates the Turtlebot's activity, sends generated occupancy maps to the path planning server, 
and uses the solution paths to direct waypoint following. This is summarized in the System Overview diagram, below. 

![alt text][system_overview]

[system_overview]: doc/img/system_overview.png "System Overview"

Below are Gazebo configurations, and a map generated by the Turtlebot. On the map is a solution path generated by PSO. 

![alt text][setup_1]

[Setup_1]: doc/img/Setup1.png "Setup 1"


![alt text][setup_1_Run_1]

[Setup_1_Run_1]: doc/img/PSO_Setup1_Run1.png "Setup 1 Run 1"

![alt text][setup_2]

[Setup_2]: doc/img/Setup2.png "Setup 2"


![alt text][setup_2_Run_2]

[Setup_2_Run_2]: doc/img/PSO_Setup2_Run2.png "Setup 2 Run 2"

#### Video Demonstrations

**Mapping**


<iframe src='undefined' frameborder='0' scrolling='no' width='100%' height='100%' style='position:absolute;top:0;left:0;' allowfullscreen></iframe>


**Path Following**

https://webmshare.com/play/ZjvLy

https://webmshare.com/play/Ddv8G

https://webmshare.com/play/6jbKB
