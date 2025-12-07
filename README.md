# Robotics-Software-Engineer || Build-My-World

- In this project, a design for a simple robot is provided, along with the design of the Gazebo world in which it will operate.

- A script is written (hello.cpp) to print a welcoming message in terminal upon launching the world.  

- This project was implemented using Ubuntu 18.04.

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

1. Got to the my_robot directory: `$ cd workspace/my_robot`.
2.  Create a build directory and compile the code:

```
$ mkdir build
$ cd build
$ cmake ..
$ make
$ export GAZEBO_PLUGIN_PATH=${GAZEBO_PLUGIN_PATH}:/home/workspace/my_robot/build
```
3. Launch the world file in Gazebo to load both the world and the plugin:
```
$ cd /home/workspace/my_robot/world
$ gazebo myworld
```
<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/b30dfb85-143e-4f5e-ad5f-e393d73a7717" />
### Troubleshooting

In case your plugins failed to load, you'll have to check and troubleshoot your error. The best way to troubleshoot errors with Gazebo is to launch it with the verbose as such:

`$ gazebo myworld --verbose`
