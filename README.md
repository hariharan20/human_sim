# Human Sim 
## The repo consists of world files for multi-actor simulation.

Steps to install
```
$ git clone https://github.com/hariharan20/human_sim
$ cd human_sim
$ git submodule update --init --recursive

```
Steps to use the docker
```
$ cd custom_dockers
$ ./build_docker.sh #Builds the docker image
$ ./run_docker.sh #Runs and creates a container of the image
```
Inside the docker image (by default the working directory should be catkin_ws):
```
$ catkin build #Build the packages
$ source devel/setup.bash #Source the workspace
```
Once the workspace has been sourced :

```
$ roslaunch human_sim_gazebo world.launch #Ref to this file for actor params
```
