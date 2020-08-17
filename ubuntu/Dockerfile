FROM ubuntu:18.04

RUN echo "deb http://mirrors.aliyun.com/ubuntu/ trusty main multiverse restricted universe" >>/etc/apt/sources.list \
&& echo "deb http://mirrors.aliyun.com/ubuntu/ trusty-backports main multiverse restricted universe" >>/etc/apt/sources.list \
&& echo "deb http://mirrors.aliyun.com/ubuntu/ trusty-proposed main multiverse restricted universe" >>/etc/apt/sources.list \
&& echo "deb http://mirrors.aliyun.com/ubuntu/ trusty-security main multiverse restricted universe" >>/etc/apt/sources.list \
&& echo "deb http://mirrors.aliyun.com/ubuntu/ trusty-updates main multiverse restricted universe" >>/etc/apt/sources.list \
&& echo "deb-src http://mirrors.aliyun.com/ubuntu/ trusty main multiverse restricted universe" >>/etc/apt/sources.list \
&& echo "deb-src http://mirrors.aliyun.com/ubuntu/ trusty-backports main multiverse restricted universe" >>/etc/apt/sources.list \
&& echo "deb-src http://mirrors.aliyun.com/ubuntu/ trusty-proposed main multiverse restricted universe" >>/etc/apt/sources.list \
&& echo "deb-src http://mirrors.aliyun.com/ubuntu/ trusty-security main multiverse restricted universe" >>/etc/apt/sources.list \
&& echo "deb-src http://mirrors.aliyun.com/ubuntu/ trusty-updates main multiverse restricted universe" >>/etc/apt/sources.list

RUN apt-get update \
&& apt-get install -y software-properties-common \
&& add-apt-repository ppa:ubuntu-toolchain-r/test \
&& apt update \
&& apt install g++-7 -y \
&& update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-7 60 --slave /usr/bin/g++ g++ /usr/bin/g++-7 \
&& update-alternatives --config gcc \
&& gcc --version \
&& g++ --version \
&& apt install ca-certificates \
&& apt-get install -y vim \
&& apt-get install -y tree \
&& apt-get install -y net-tools \
&& apt-get install -y git \
&& apt-get install -y nginx \
&& apt-get install -y redis-server \
&& apt-get install -y python3.7 \
&& apt-get install -y python3-pip \
&& apt-get install -y python-pip python-dev build-essential 