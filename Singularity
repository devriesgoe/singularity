Bootstrap: docker
From: ubuntu:latest

%help

Test container for dask environment using ipyparallel


%post

apt-get -y update
apt-get -y install python3-pip

pip3 install virtualenv
pip3 install jupyter
pip3 install ipyparallel
pip3 install numpy scipy matplotlib
pip3 install dask[complete]

%environment

XDG_RUNTIME_DIR=""
PATH=${PATH}:${LSF_BINDIR}
