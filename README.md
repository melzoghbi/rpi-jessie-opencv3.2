# rpi-jessie-opencv3.2

This is a docker file that creates a container image for Raspberry Pi Zero (Single Core) with Raspbian Jessie and OpenCV 3.2.


This image is an extension of the resin.io Raspberry Pi base image (Jessie); We added OpenCV 3.2 libraries and python 2.7 & 3.0 bindings added. 

The installation steps is based upon instructions from pyimage search article below:
http://www.pyimagesearch.com/2016/04/18/install-guide-raspberry-pi-3-raspbian-jessie-opencv-3/


## Why to use this docker image
Building OpenCV 3.2 lib on a Raspberry Pi Zero W takes more than 15 hours! This is after i tried to build it with multiple cores as mentioned on the above article. So i decided to build this docker file to make it easier to build and run docker image with OpenCV 3.2 on a Raspberry Pi Zero W running Raspbian Jessie OS.


To build:

    docker build -ti rpi-jessie-opencv3.2 .
