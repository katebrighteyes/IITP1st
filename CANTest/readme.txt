sudo apt-get update -y

sudo apt-get install -y can-utils

sudo modprobe gs_usb
sudo modprobe can_dev
sudo ip link set can0 type can bitrate 500000
sudo ifconfig can0 up

ifconfig can0


candump can0

cangen can0 -v
