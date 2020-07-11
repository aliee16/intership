# intership
               **FIRST TASK**
Aftre downlaod Virtualbox and insall Ubuntu-20.04 on it from these links:
[https://www.virtualbox.org/wiki/Downloads](url)
[https://ubuntu.com/download/desktop](url) 

**Install Ros**

**Step 1** — Set up ROS Noetic repo for Ubuntu 20.04:
echo "deb http://packages.ros.org/ros/ubuntu focal main" | sudo tee /etc/apt/sources.list.d/ros-focal.list

![Screenshot (37)](https://user-images.githubusercontent.com/67034346/87220312-5e588d00-c36b-11ea-9d1d-c811f0045e12.png)


**Step 2** — Add official ROS keyring:
sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654

![Screenshot (38)](https://user-images.githubusercontent.com/67034346/87220320-6fa19980-c36b-11ea-9d77-492547824af3.png)

The second way if you has not internet :

curl -sSL 'http://keyserver.ubuntu.com/pks/lookup?op=get&search=0xC1CF6E31E6BADE8868B172B4F42ED6FBAB17C654' | sudo apt-key add -


![Screenshot (39)](https://user-images.githubusercontent.com/67034346/87220327-82b46980-c36b-11ea-9af4-692590aa34d0.png)

If you see output “OK”, the key is successfully added.


**Step 3** — Update ROS package index:
sudo apt update

![Screenshot (40)](https://user-images.githubusercontent.com/67034346/87220334-89db7780-c36b-11ea-84bd-22e20cab9511.png)


**Step 4** — Install ROS Noetic package:
sudo apt install ros-noetic-desktop

![Screenshot (41)](https://user-images.githubusercontent.com/67034346/87220348-9bbd1a80-c36b-11ea-949e-9e046a22018e.png)

there are four packages but i choose the desktop   


**Set up ROS Noetic environment**
source /opt/ros/noetic/setup.bash


In case you are using zsh instead of bash, run the follow command instead:
echo "source /opt/ros/noetic/setup.zsh" >> ~/.zshrc

**Verify Noetic installation**
We can also verify the installation by running (roscore )

![Screenshot (42)](https://user-images.githubusercontent.com/67034346/87220385-e179e300-c36b-11ea-9a8d-61b81d39c1e6.png)
