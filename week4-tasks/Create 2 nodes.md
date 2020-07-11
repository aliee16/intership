


![image](https://user-images.githubusercontent.com/67034346/87222283-3b35d980-c37b-11ea-8388-02ee5b2bd808.png)

> Let's create and build a catkin workspace:
`$ mkdir -p ~/catkin_ws/src`
`$ cd ~/catkin_ws/`
`$ catkin_make`

![Screenshot (44)](https://user-images.githubusercontent.com/67034346/87223027-ff524280-c381-11ea-9e68-bc464f99b0e1.png)
![Screenshot (45)](https://user-images.githubusercontent.com/67034346/87223030-15f89980-c382-11ea-8535-a9527597ec52.png)

>source your new setup.*sh file:
`$ source devel/setup.bash`

>To know the path of the package run this:
`$ echo $ROS_PACKAGE_PATH`

![Screenshot (61)](https://user-images.githubusercontent.com/67034346/87223050-4e987300-c382-11ea-8c7d-4f8faa9a9a27.png)

![image](https://user-images.githubusercontent.com/67034346/87222278-2eb18100-c37b-11ea-8c98-b7fd23e7a97c.png)

>let us start from src so :
`$ cd ~/catkin_ws/src`

>to create a new package called 'ali_task'
`$ catkin_create_pkg ali_task std_msgs rospy `

![Screenshot (49)](https://user-images.githubusercontent.com/67034346/87223067-725bb900-c382-11ea-911a-6bcc957527ea.png)

>To add the workspace to your ROS environment you need to source the generated setup file:
`$ cd ~/catkin_ws`
`$ catkin_make`
`$ . ~/catkin_ws/devel/setup.bash`

![Screenshot (50)](https://user-images.githubusercontent.com/67034346/87223108-d7afaa00-c382-11ea-9c95-569a313f6b4f.png)

![image](https://user-images.githubusercontent.com/67034346/87222297-4d177c80-c37b-11ea-8fd5-05d2f9e3ac3e.png)

> start from pachage:

`$ roscd ali_task`

> First lets create a 'scripts' folder to store our Python scripts in:

`$ mkdir scripts`
`$ cd scripts`

![Screenshot (52)](https://user-images.githubusercontent.com/67034346/87223190-805e0980-c383-11ea-9f15-c6b3a9c44612.png)


>  download the example script talker.py as(Publisher) to your new scripts directory and make it executable:

```
$ wget https://raw.github.com/ros/ros_tutorials/kinetic-devel/rospy_tutorials/001_talker_listener/talker.py
$ chmod +x talker.py
```

![Screenshot (53)](https://user-images.githubusercontent.com/67034346/87223216-cca94980-c383-11ea-9dff-8e49871f2205.png)



> Download the listener.py as(Subscriber) file into your scripts directory:

```
$ wget https://raw.github.com/ros/ros_tutorials/kinetic-devel/rospy_tutorials/001_talker_listener/listener.py
$ chmod +x listener.py
```

![Screenshot (55)](https://user-images.githubusercontent.com/67034346/87223230-e34fa080-c383-11ea-9aea-d7f639e0b789.png)

**Then you can edit on them :**

![Screenshot (62)](https://user-images.githubusercontent.com/67034346/87223303-56f1ad80-c384-11ea-984a-5ba4c44604db.png)
![Screenshot (61)](https://user-images.githubusercontent.com/67034346/87223304-5822da80-c384-11ea-81b4-b09f95992424.png)

**To run them you have to make `roscore `running** 
![Screenshot (60)](https://user-images.githubusercontent.com/67034346/87223342-cb2c5100-c384-11ea-910e-1e0bdaa7af42.png)



 Then make them run:

![Screenshot (58)](https://user-images.githubusercontent.com/67034346/87223345-d1223200-c384-11ea-874b-0fcca62c592a.png)
![Screenshot (59)](https://user-images.githubusercontent.com/67034346/87223346-d2535f00-c384-11ea-8088-49d65981418d.png)


