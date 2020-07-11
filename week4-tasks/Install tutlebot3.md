
![image](https://user-images.githubusercontent.com/67034346/87229953-2aa25500-c3b5-11ea-9d29-b582764c7719.png)

> Let us start from src in workspace and install package turtlebo3:

`$ cd ~/catkin_ws/src`
`$ git clone https://github.com/ROBOTIS-GIT/turtlebot3.git`
`$ cd ~/catkin_ws/`
`$ catkin_make`


![image](https://user-images.githubusercontent.com/67034346/87229958-342bbd00-c3b5-11ea-8e18-86b847a34fd7.png)

> Then downlaod simulation:

`$ cd ~/catkin_ws/src`
`$ git clone https://github.com/ROBOTIS-GIT/turtlebot3_simulations.git`
`$ cd ~/catkin_ws/`
`$ catkin_make`
`$ source devel/setup.bash`



![image](https://user-images.githubusercontent.com/67034346/87229964-39890780-c3b5-11ea-9920-ac0c0e206854.png)

> To run the simulation we have to launch the last two line separately in each terminal and we choose the model burger:

```
$ export TURTLEBOT3_MODEL=burger
$ roslaunch turtlebot3_fake turtlebot3_fake.launch ##This launches Rviz to start simulation
$ roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch ## this lauches the control to move the Robot execute in a new terminal 
```

![Screenshot (68)](https://user-images.githubusercontent.com/67034346/87230280-8372ed00-c3b7-11ea-98d0-77e6507cae56.png)
