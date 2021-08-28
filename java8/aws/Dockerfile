# sxlehua/java8:aws
# docker build -t sxlehua/java8:aws .
FROM amazoncorretto:8

# MAINTAINER
MAINTAINER sxlehua "sxlehua@qq.com"

# 增加常用软件
RUN yum install -y procps net-tools && yum clean all

# 设置时区
RUN echo "Asia/Shanghai" > /etc/timezone \
&& ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime
