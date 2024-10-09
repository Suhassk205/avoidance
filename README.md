Simulation of PX4 drone with Obstacle Avoidance in Gazebo.

This contains the maze model and the edited launch file used in the simulation.

-----------------------------------------------------------------------------------------------------------------------------------

Demonstration:It can be found in my youtube channel.
Link for the video-https://youtu.be/c024dl6Hasg?si=jO0Ivsi5ZXRoEpeS

Installation and setup can be found at https://github.com/Jaeyoung-Lim/avoidance.

-----------------------------------------------------------------------------------------------------------------------------------

Waypoint Navigation with Gazebo Simulator
This project demonstrates how a drone autonomously navigates through a series of GPS waypoints in a simulated environment using ROS (Robot Operating System) and Gazebo. The simulation features a maze model where the drone plans and follows a path from start to finish efficiently.



Project Overview
The goal of this project is to introduce key concepts in drone flight autonomy, including GPS waypoint navigation and path planning in the Gazebo simulator. ROS is used for controlling the drone and integrating sensor data like GPS and IMU (Inertial Measurement Unit) to ensure stable and accurate navigation through the maze model.



Key Features
1.Autonomous Navigation: The drone autonomously follows a series of predefined GPS waypoints.
2.Path Planning: Efficient path planning minimizes travel time and ensures smooth transitions between waypoints.
3.ROS Integration: Utilizes relevant ROS packages for drone control, GPS handling, and communication with the Gazebo simulator.
4.Simulation Environment: The Gazebo simulator is used to create the virtual environment, including a custom maze model where the drone navigates.



Repository Structure
1.avoidance/
   *Edited_launch_file/
       -global_planner_sitl_mavros.launch: This launch file configures the SITL (Software In The Loop) for MAVROS and the global planner, enabling 
        the drone to navigate through waypoints autonomously.
2.maze_model/
   *model.config: Defines the configuration for the maze model used in the Gazebo simulation.
   *model.sdf: The SDF (Simulation Description Format) file that specifies the physical structure and properties of the maze.
3.README.md: Documentation providing instructions and project overview.



Setup Instructions
Follow these steps to set up and run the simulation on your local machine:

1. Install ROS and Gazebo
Make sure you have ROS Noetic and Gazebo installed. Follow this tutorial for installation instructions.

2. Clone the Repository
bash-git clone https://github.com/your-username/waypoint-navigation-simulator.git
bash-cd waypoint-navigation-simulator

4. Install Dependencies
Install all required ROS packages, including mavros, ros_control, and gazebo_ros, using the following command:
bash-sudo apt-get install ros-noetic-mavros ros-noetic-ros-control ros-noetic-gazebo-ros

6. Build the Workspace
Once the repository is cloned, build the ROS workspace:
bash-catkin_make
bash-source devel/setup.bash

5. Launch the Simulation
To start the drone simulation in the maze, run the provided launch file:
bash-roslaunch avoidance global_planner_sitl_mavros.launch
This will launch the Gazebo simulator with the maze model and initiate the drone's waypoint navigation sequence.



Task Objectives
Autonomous Navigation: The drone will autonomously follow GPS waypoints within the maze.
Path Planning: The system will implement an efficient path planning algorithm to minimize the drone’s travel time while ensuring smooth navigation.
ROS Integration: The navigation system uses ROS to control the drone and interact with the Gazebo simulation.



Simulation Demo
Check out a demo video showing the drone navigating through the maze model in Gazebo.
Link for the video-https://youtu.be/c024dl6Hasg?si=jO0Ivsi5ZXRoEpeS
