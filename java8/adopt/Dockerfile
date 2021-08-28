# sxlehua/java8:adopt
# docker build -t sxlehua/java8:adopt .
FROM adoptopenjdk/openjdk8:centos

# MAINTAINER
MAINTAINER sxlehua "sxlehua@qq.com"

# 增加常用软件
RUN yum install -y net-tools && yum clean all

# 设置时区
RUN echo "Asia/Shanghai" > /etc/timezone \
&& ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime

