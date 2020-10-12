
FROM nvidia/cuda:10.2-cudnn7-devel-ubuntu18.04

COPY ./keyboard /etc/default/keyboard
WORKDIR /code
ENV DEBIAN_FRONTEND=noninteractive
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
	
#RUN wget https://developer.download.nvidia.com/compute/cuda/repos/ubuntu1804/x86_64/cuda-repo-ubuntu1804_10.0.130-1_amd64.deb

#RUN wget https://dockeryolov4.s3-eu-west-1.amazonaws.com/libcudnn7_7.6.4.38-1%2Bcuda10.0_amd64.deb

#RUN wget https://dockeryolov4.s3-eu-west-1.amazonaws.com/libcudnn7-dev_7.6.4.38-1%2Bcuda10.0_amd64.deb

#RUN wget https://dockeryolov4.s3-eu-west-1.amazonaws.com/libcudnn7-doc_7.6.4.38-1%2Bcuda10.0_amd64.deb



#RUN sudo dpkg -i cuda-repo-ubuntu1804_10.0.130-1_amd64.deb
#RUN sudo apt-key adv --fetch-keys https://developer.download.nvidia.com/compute/cuda/repos/ubuntu1804/x86_64/7fa2af80.pub && sudo apt-get update && sudo apt-get install -y cuda


#RUN sudo dpkg -i libcudnn7_7.6.4.38-1+cuda10.0_amd64.deb
#RUN sudo dpkg -i libcudnn7-dev_7.6.4.38-1+cuda10.0_amd64.deb
#RUN sudo dpkg -i libcudnn7-doc_7.6.4.38-1+cuda10.0_amd64.deb

RUN sudo git clone https://github.com/AlexeyAB/darknet.git




