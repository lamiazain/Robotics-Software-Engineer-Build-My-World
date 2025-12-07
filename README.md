# Robotics-Software-Engineer || Build-My-World

In this project, a design of a simple robot is provided with the design of the environment.

A script is written (hello.cpp) to print a welcoming message upon launching the project.  

This project was implemented using Ubuntu 18.04.

## Project structure
```
my_robot/                             # Build My World Project 
├── model/                            # Model files 
│   ├── building/
│   │   ├── model.config
│   │   ├── model.sdf
│   ├── robot/
│   │   ├── model.config
│   │   ├── model.sdf
│
├── script/                           # Gazebo World plugin C++ script
│   ├── hello.cpp
│
├── world/                            # Gazebo main world containing models
│   ├── myworld.world
│
└── CMakeLists.txt                    # CMake configuration and library linking
```
## Steps to run the project:

1. Got to the workspace: `$ cd workspace`
2. Build the package: `$ catkin_make`
3. Source the setup.bash file: `$ source setup.bash`
4. 
