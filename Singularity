Bootstrap: docker
From: ubuntu:latest

%help

Test container for dask environment


%post

apt-get -y update
apt-get -y install python3-pip net-tools

pip3 install --upgrade pip
pip3 install jupyter
pip3 install numpy scipy matplotlib
pip3 install dask[complete]


%environment

XDG_RUNTIME_DIR=""
PATH=${PATH}:${LSF_BINDIR}