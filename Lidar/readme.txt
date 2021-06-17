# Camsensor 라이다인 경우

cd catkin_ws/src/
ls

ls /dev/tty*
ll /dev/ttyUSB0
sudo chmod 777 /dev/ttyUSB0 

git clone https://github.com/Vidicon/camsense_driver
ls
cd ..
catkin_make
source ./devel/setup.bash
roslaunch camsense_driver view.launch 

---------------------------------------------------------------
# lds01 라이다인 경우

참고 : http://wiki.ros.org/hls_lfcd_lds_driver

cd catkin_ws/src/
ls

ls /dev/tty*
ll /dev/ttyUSB0
sudo chmod 777 /dev/ttyUSB0 

git clone https://github.com/ROBOTIS-GIT/hls_lfcd_lds_driver
ls
cd ..
catkin_make
source ./devel/setup.bash
roslaunch hls_lfcd_lds_driver view_hlds_laser.launch

* 참고 : fixed frame : laser

---------------------------------------------------


* 참고 : http://wiki.ros.org/velodyne/Tutorials/Getting%20Started%20with%20the%20Velodyne%20VLP16

git clone https://github.com/ros-drivers/velodyne.git
ls
cd ..
catkin_make
source ./devel/setup.bash
roslaunch velodyne_pointcloud VLP16_points.launch


