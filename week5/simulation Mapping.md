
**simulation Mapping Slam by ros kinetic**

> let us start open three terminal in each terminal we have do this:
 
`$ cd catkin_ws`

`$ export TURTLEBOT3_MODEL=burger`

> first terminal open gazbo:

`$ roslaunch turtlebot3_gazebo turtlebot3_world.launch
`

![‏‏لقطة الشاشة (1)](https://user-images.githubusercontent.com/67034346/87856942-5c726900-c92b-11ea-8bed-7cfa40599db0.png)


> seconed terminal open slam gmappin:

`$ roslaunch turtlebot3_slam turtlebot3_slam.launch slam_methods:=gmapping
`

![‏‏لقطة الشاشة (2)](https://user-images.githubusercontent.com/67034346/87856946-63997700-c92b-11ea-81e0-8169f7cb777e.png)


> the last terminal open the control keys:

`$ roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch 
`

then you can save the map : 

`$ rosrun map_server map_saver -f ~/map`

the result : 

![‏‏لقطة الشاشة (3)](https://user-images.githubusercontent.com/67034346/87856976-9e9baa80-c92b-11ea-8b27-2cc8b437fce7.png)
