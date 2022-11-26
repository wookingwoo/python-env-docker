FROM ubuntu:22.04

MAINTAINER wookingwoo

#사용자 입력 요구 방지
ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get -y update

# Install python 3.11
RUN apt-get -y install software-properties-common
RUN add-apt-repository -y ppa:deadsnakes/ppa
RUN apt-get -y install python3.11
RUN apt-get -y install python3-pip
RUN apt-get -y install python3.11-distutils
# End Of Install python 3.11

CMD ["python3"]
