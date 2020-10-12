# From the NVIDIA repository - Download an UBUNTU docker image that has already installed 
# the CUDA and cuDNN library versions needed to run YOLO
FROM nvidia/cuda:10.2-cudnn7-devel-ubuntu18.04

#Copy the file keyboard (from the current directory in the local machine) to the 
#folder /etc/default/keyboard that will be created in the Docker container
COPY ./keyboard /etc/default/keyboard

# Create a folder named code in the root directory and enter it (like mkdir /code + cd /code)
WORKDIR /code

#This flag ensures that no prompts are shown when the installation is performed
ENV DEBIAN_FRONTEND=noninteractive

# Packages to be installed
RUN  apt-get update && apt-get install -y \
	sudo\
	--reinstall keyboard-configuration\
	wget\
	python3-pip\
    	python3-opencv\
	libopencv-dev\
	libomp-dev\
	python-qt4 \
    	python-pyside \
    	python3-pip \
    	python3-pyqt5\
	nano\
	git\
    	cmake 
	
RUN pip3 install\
	scikit-learn\
	tqdm\
	numpy\
	jupyter\
	pandas
	
# Clone the darknet Github in the current folder	
RUN sudo git clone https://github.com/AlexeyAB/darknet.git




