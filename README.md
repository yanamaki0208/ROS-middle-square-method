# 2020 Robot system task2 
# ROS-middle-square-method（平方採中法）  

This is a repository of  that middle-square method have been converted to ROS.

# DEMO
This is a shot of random numbers being generated.　↓　![image](https://user-images.githubusercontent.com/66021066/103771582-5607b300-506b-11eb-9dab-7a3d909c44f7.png)
This is a link to a demo video　→　https://www.youtube.com/watch?v=T2Y9UUCg_V8&feature=youtu.be

# Requirement  
*OS Ubuntu 20.04LTS  
*ROS Noetic Ninjemys  

# Usage
## Step 1.
#### terminal 1

*turn on the communication between ROS nodes.  
`ubuntu@ubuntu:~$ roscore`  

#### terminal 2

*move directory  
`ubuntu@ubuntu:~$ cd catkin_ws`  
`ubuntu@ubuntu:~/catkin_ws$ cd src`  

*copy the repository  
`ubuntu@ubuntu:~/catkin_ws/src$ git clone https://github.com/yanamaki0208/ROS-middle-square-method.git`  

*move directory  
`ubuntu@ubuntu:~/catkin_ws/src$ cd ROS-middle-spuare-method`  
`ubuntu@ubuntu:~/catkin_ws/src/ROS-middle-square-method$ cd script`  

*give execution privileges to all users  
`ubuntu@ubuntu:~/catkin_ws/src/ROS-middle-square-method/script$ chmod +x heihoupub.py`  

#### terminal 3  

*move directory  
`ubuntu@ubuntu:~$ cd catkin_ws`  

*build this package  
`ubuntu@ubuntu:~/catkin_ws$ catkin_make`  

*move directory
`ubuntu@ubuntu:~/catkin_ws$ cd src`  
`ubuntu@ubuntu:~/catkin_ws/src$ cd ROS-middle-square-method`  
`ubuntu@ubuntu:~/catkin_ws/src/ROS-middle-square-method$ cd script`  

*give execution privileges to all users  
`ubuntu@ubuntu:~/catkin_ws/src/ROS-middle-square-method/script$ chmod +x heihousub.py`  

#### terminal 4  

*I won't do anything  
`ubuntu@ubuntu:~$` 

## Step 2.
#### terminal 2  

*move nodes that perform calculations and produce information  
`ubuntu@ubuntu:~/catkin_ws/src/ROS-middle-square-method/script$ rosrun ROS-middle-square-method heihoupub.py`  

#### terminal3  

*move the nodes that pick up the information  
`ubuntu@ubuntu:~/catkin_ws/src/ROS-middle-square-method/script$ rosrun ROS-middle-square-method heihousub.py`  

#### terminal4  

*show communication between nodes  
`ubuntu@ubuntu:~$ rostopic echo /twice`  

# Note

The smaller the initial value s1 is, the faster the random number converges to zero.

# Author

* Masaki Yara and Ryuichi Ueda  
* Chiba Institute of Technology  
* masaki.yara@gmail.com  

# License

"middle-square-method" is under [GNU General Public License v3.0](https://ja.wikipedia.org/wiki/GNU_General_Public_License#%E3%83%90%E3%83%BC%E3%82%B8%E3%83%A7%E3%83%B33).
