FROM dockerhub.io/centos:centos7
MAINTAINER garethahealy (https://github.com/garethahealy/)

RUN sudo yum makecache && \
     yum install -y deltarpm && \
     yum install -y epel-release && \
     yum update -y && \
     yum install -y gcc kernel-devel make && \
     yum install -y java-1.8.0-openjdk.x86_64 java-1.8.0-openjdk-devel.x86_64 && \
     yum install -y curl wget vim zip unzip tar telnet bc git && \
     yum install -y lokkit sshpass nmap apache-maven libaio && \
     yum clean all

