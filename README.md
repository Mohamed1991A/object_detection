# object_detection
# Mohamed BEN ALI --- BIG DATA 
les étapes d'installation suivantes :
1st : une distribution de linux Debian ou redhat 
# Ubuntu_16.04/18.04/18.10     ect
2nd : $ git clone https://github.com/Mohamed1991A/object_detection1.git
# avoir les packages suivantes sur votre linux (exp: ubuntu)
----- packages dependencies
----------install
**********************************
RUN 
apt-get update && \
    apt-get install -y \
    build-essential \
    cmake \
    git \
    wget \
    unzip \
    yasm \
    pkg-config \
    curl 

apt-get install -y \
    libswscale-dev libtbb2 libtbb-dev libjpeg-dev libpng-dev libtiff-dev \
    libjasper-dev libavformat-dev libpq-dev libxine2-dev libglew-dev \
    libtiff5-dev zlib1g-dev libjpeg-dev libpng12-dev libjasper-dev \
    libavcodec-dev libavformat-dev libavutil-dev libpostproc-dev \
	libswscale-dev libeigen3-dev libtbb-dev libgtk2.0-dev 
    # libcudnn7=7.1.4.18-1+cuda9.0 

apt-get install -y \
    python3-dev \
    python3-numpy \
    python3-pip

# Python dependencies
RUN 
pip3 --no-cache-dir install \
    numpy \
    hdf5storage \
    h5py \
    scipy \
    py3nvml
pip3 install matplotli
# Install tensorflow
RUN 
pip3 --no-cache-dir install tensorflow-gpu==1.13.0
# install open cv4
# see this link
https://www.pyimagesearch.com/2018/08/15/how-to-install-opencv-4-on-ubuntu/

