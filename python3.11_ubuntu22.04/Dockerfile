FROM ubuntu:22.04

MAINTAINER wookingwoo

#사용자 입력 요구 방지
ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get -y update
RUN apt-get -y install software-properties-common
RUN add-apt-repository -y ppa:deadsnakes/ppa

# Installing Python 3.11
RUN apt-get -y install python3.11

# Making Python 3.11 the default version.
RUN update-alternatives --install /usr/bin/python python /usr/bin/python3.11 1

# Installing supporting packages for Python 3.11
RUN apt-get -y update
RUN apt-get -y install python3-pip python3.11-dev python3.11-venv python3.11-distutils python3.11-gdbm python3.11-tk python3.11-lib2to3

# CMD ["python3"]
