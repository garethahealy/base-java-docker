FROM docker.io/centos:centos7
MAINTAINER garethahealy (https://github.com/garethahealy/)

LABEL Name="base-java-docker" \
    Vendor="com.garethahealy" \
    Version="1.0.2"
    License="Apache License, Version 2.0"

RUN yum makecache && \
     yum install -y deltarpm && \
     yum install -y epel-release && \
     yum update -y && \
     yum install -y gcc kernel-devel make && \
     yum install -y java-1.8.0-openjdk.x86_64 java-1.8.0-openjdk-devel.x86_64 && \
     yum install -y curl wget vim zip unzip tar telnet bc git && \
     yum install -y lokkit sshpass nmap libaio && \
     yum clean all

RUN wget -O /etc/yum.repos.d/epel-apache-maven.repo http://repos.fedorapeople.org/repos/dchen/apache-maven/epel-apache-maven.repo && \
     yum install -y apache-maven && \
     yum clean all
