# Prerequisites
You have to disable the automatic management of camera led in `/boot/config.txt`.  
```bash
$ sudo sh -c 'echo "disable_camera_led=1" >> /boot/config.txt' 
$ sudo reboot
```
# Quickly start
## Download the Raspberrypi library
```bash
git clone https://github.com/ArduCAM/RaspberryPi.git
```
![Alt text](https://github.com/ArduCAM/RaspberryPi/blob/master/Multi_Camera_Adapter/Multi_Adapter_Board_2Channel/data/download_code.png)

## Shell version

This shell script is used to test each camera 
* Run the script
```bash
cd RaspberryPi/Multi_Camera_Adapter/Multi_Adapter_Board_2Channel/shell

sudo chmod +x pi_zero_cam.sh

sudo ./pi_zero_cam.sh
```
* Running Demo
![Alt text](https://github.com/ArduCAM/RaspberryPi/blob/master/Multi_Camera_Adapter/Multi_Adapter_Board_2Channel/data/shell_demo.png)

## C++ version code

This demo supports Both cameras display at the same time

* Install the opencv library
```Bash
sudo apt-get install libopencv-dev
```
* Compile and run
```Bash
cd RaspberryPi/Multi_Camera_Adapter/Multi_Adapter_Board_2Channel/c++/

sudo make

sudo ./pi_zero_cam
```
* Runing Demo
![Alt text](https://github.com/ArduCAM/RaspberryPi/blob/master/Multi_Camera_Adapter/Multi_Adapter_Board_2Channel/data/demo.png)