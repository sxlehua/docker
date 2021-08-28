# sxlehua/java8:openjdk
# docker build -t sxlehua/java8:openjdk .
# docker tag sxlehua/java8:openjdk sxlehua/java8
#FROM openjdk:8
FROM openjdk:8-oraclelinux7

# MAINTAINER
MAINTAINER sxlehua "sxlehua@qq.com"

# 修改源
# RUN	sed -i 's/deb.debian.org/mirrors.aliyun.com/g' /etc/apt/sources.list

# 增加常用软件
# RUN	apt-get update; \
#	apt-get install -y --no-install-recommends \
#		net-tools \
#	; \
#	rm -rf /var/lib/apt/lists/*
RUN yum install -y net-tools iputils vi && yum clean all

# 设置时区
RUN echo "Asia/Shanghai" > /etc/timezone \
&& ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime
