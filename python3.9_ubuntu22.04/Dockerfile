FROM ubuntu:22.04

MAINTAINER wookingwoo

#사용자 입력 요구 방지
ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get -y update
RUN apt-get -y install software-properties-common
RUN add-apt-repository -y ppa:deadsnakes/ppa

# Installing Python 3.9
RUN apt-get -y install python3.9

# Making Python 3.9 the default version.
RUN update-alternatives --install /usr/bin/python python /usr/bin/python3.9 1
RUN update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.9 1

# Installing supporting packages for Python 3.9
RUN apt-get -y install python3-pip python3.9-dev python3.9-venv python3.9-distutils python3.9-gdbm python3.9-tk python3.9-lib2to3

# CMD ["python3"]
