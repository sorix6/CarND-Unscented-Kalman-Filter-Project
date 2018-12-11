# Extended Kalman Filter Project 

This project consists of using an Unscented Kalman filter to estimate the state of a moving object with noisy Lidar and Radar measurements.

The project consists of the following steps:
* Initializing the Unscented Kalman filter
* Predicting where the object will be after a time lapse of Δt
* Updating the object position based on the measurements received from the sensors
* Tunning the process noise


The code has been developed on an Ubuntu 16.04 Virtual Machine running on Oracle VM VirtualBox.
The Term 2 Simulator has been run on the same virtual machine.

The executable file compiled for this project can be found in the folder **build**, under the name **UnscentedKF**


The pictures below, shows print-screen of the simulator for the two datasets.
* The red circles represent the Lidar measurements 
* The blue circles represent the radar measurements and the arrow points in the direction of the observed angle
* The green triangles represent the estimation markers 

Dataset 1 | Dataset 2  
------------ | ------------- 
![Simulator print-screen](https://raw.githubusercontent.com/sorix6/CarND-Unscented-Kalman-Filter-Project/master/images/rmse_d1.PNG) | ![Simulator print-screen](https://raw.githubusercontent.com/sorix6/CarND-Unscented-Kalman-Filter-Project/master/images/rmse_d2.PNG) 


Consistency checks have been done and the images below provide the graphs for the NIS radar and lidar, respectively:

NIS Radar | NIS Lidar 
------------ | ------------- 
![Simulator print-screen](https://raw.githubusercontent.com/sorix6/CarND-Unscented-Kalman-Filter-Project/master/images/nis_radar.PNG) | ![Simulator print-screen](https://raw.githubusercontent.com/sorix6/CarND-Unscented-Kalman-Filter-Project/master/images/nis_lidar.PNG) 


Tests have been also run by using alternatively, only radar or lidar measurements. Some results can be seen below: 

Radar only | Lidar only
------------ | ------------- 
![Simulator print-screen](https://raw.githubusercontent.com/sorix6/CarND-Unscented-Kalman-Filter-Project/master/images/radar_only.PNG) | ![Simulator print-screen](https://raw.githubusercontent.com/sorix6/CarND-Unscented-Kalman-Filter-Project/master/images/lidar_only.PNG) 


The process noise standard deviation longitudinal acceleration in m/s^2 (std_a_) and the process noise standard deviation yaw acceleration in rad/s^2(std_yawdd_) have been chosen through testing. The values have been set as follows:
* std_a_ = 2 m/s^2
* std_yawdd_ = M_PI/6 rad/s^2









