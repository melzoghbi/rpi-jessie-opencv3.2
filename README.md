# Raspbian Jessie with OpenCV 3.2

This is a docker file that creates a container on a Raspberry Pi Zero (Single Core) with Raspbian Jessie with OpenCV 3.2 installed.


This image is an extension of the resin.io Raspberry Pi base image (Jessie); We added OpenCV 3.2 library with python 2.7 & 3.0 bindings added. 

The installation steps is based upon instructions from pyimage search article below:
http://www.pyimagesearch.com/2016/04/18/install-guide-raspberry-pi-3-raspbian-jessie-opencv-3/


## Why would i use this docker image than install everything manually?

Based on my experience on following the above steps to install OpenCV 3.2 on a Raspberry Pi Zero W, It took around 15 hours to build OpenCV 3.2! This is after i tried to build it with multiple cores as mentioned on the above article which did not work in this case.

For this reason, I decided to create this docker file to make it easier to build and run docker Jessie image with OpenCV 3.2 on a Raspberry Pi Zero W.


## How to use a docker file on a Raspberry Pi Zero?

1) Open the terminal window on your RPI Zero.

2) Clone this git hub repo on your RPI by executing below command:

```
git clone https://github.com/melzoghbi/rpi-jessie-opencv3.2.git
```

2) Navigate to the directory where the repo has been downloaded:

```
cd rpi-jessie-opencv3.2
```

3) Build the image from the docker file:

```
docker build .
```

4) When the docker completes building the image, you can run a container of this image!



Enjoy!



