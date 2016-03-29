FROM ubuntu:latest

MAINTAINER Dhia Eddine Saidi <dhiasaidi.ensit@gmail.com>

RUN apt-get -y update \
    && apt-get install -y python python-pip \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

RUN pip install robotframework==2.9
RUN pip install robotframework-selenium2library==1.7.2
RUN pip install robotframework-sofrecomappiumlibrary==1.0.1
RUN pip install robotframework-faker==3.0.0

RUN     mkdir /robot
VOLUME  /robot
WORKDIR /robot
