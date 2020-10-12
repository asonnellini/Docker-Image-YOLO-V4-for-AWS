# Docker-Image-YOLO4-for-AWS

Have you tried to install YOLO V4 on your laptop enabling GPU computation? 

If yes, I think you may have faced some challenge in terms of dependencies and amount of Disk space.

In this repository I briefly show how to create a docker image having YOLO V4 that can run on an AWS Px EC2. 
From now on, having access to YOLO V4 will be as easy as running a Docker image.

I plan in the coming weeks to further improve this Docker image to have a ready-to-go YOLO V4 docker container.

I will make use of the [YOLO4 darknet implementation](https://github.com/AlexeyAB/darknet). 

Special thanks to the [author of this youtube video](https://www.youtube.com/watch?v=B8ZJXKG8AOw&t=491s) who pointed me to the NVIDIA docker repository where I could find an Ubuntu docker image with all NVIDIA libraries needed for YOLO V4 installed.