
cd catkin_ws/src/
ls

ls /dev/tty*
ll /dev/ttyUSB0
sudo chmod 777 /dev/ttyUSB0 

git clone https://github.com/Vidicon/camsense_driver
30  ls
cd ..
catkin_make
source ./devel/setup.bash
roslaunch camsense_driver view.launch 

