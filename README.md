# Extended Kalman Filter 

## Intro

This project consists in the implementation of a extented Kalman filter in C++. Extended Kalman Filter (EKF) is a nonlinear version of the Kalman Filter, which is an algorithm that uses a series of measurements observed over time and help us to track the position of objects.

The process is as follows. We predict the position of the object after a period of time Δt, and then we compare that prediction with what the sensor (Radar or Lidar) measurement provides. The Kalman filter will put more weight on either the predicted location or the measured location depending on the uncertainty of each value. The flow can be seen in this diagram:

![image1](./assets/flow.png)


## Requirements

This project involves the Term 2 Simulator which can be downloaded [here](https://github.com/udacity/self-driving-car-sim/releases)

This repository includes two files that can be used to set up and install [uWebSocketIO](https://github.com/uWebSockets/uWebSockets) for either Linux or Mac systems. For windows you can use either Docker, VMware, or even [Windows 10 Bash on Ubuntu](https://www.howtogeek.com/249966/how-to-install-and-use-the-linux-bash-shell-on-windows-10/) to install uWebSocketIO. 

## How to run the code

Once requirements are fullfield, you can run the code following the next steps:

1. mkdir build
2. cd build
3. cmake ..
4. make
5. ./ExtendedKF


## Other Important Dependencies

* cmake >= 3.5
  * All OSes: [click here for installation instructions](https://cmake.org/install/)
* make >= 4.1
  * Linux: make is installed by default on most Linux distros
  * Mac: [install Xcode command line tools to get make](https://developer.apple.com/xcode/features/)
  * Windows: [Click here for installation instructions](http://gnuwin32.sourceforge.net/packages/make.htm)
* gcc/g++ >= 5.4
  * Linux: gcc / g++ is installed by default on most Linux distros
  * Mac: same deal as make - [install Xcode command line tools](https://developer.apple.com/xcode/features/)
  * Windows: recommend using [MinGW](http://www.mingw.org/)

## Basic Build Instructions

1. Clone this repo.
2. Make a build directory: `mkdir build && cd build`
3. Compile: `cmake .. && make` 
   * On windows, you may need to run: `cmake .. -G "Unix Makefiles" && make`
4. Run it: `./ExtendedKF `


## Code Style

This code is intented to follow the  [Google's C++ style guide](https://google.github.io/styleguide/cppguide.html).

