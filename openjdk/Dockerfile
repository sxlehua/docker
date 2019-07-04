# sxlehua/java
FROM openjdk:8-alpine

# MAINTAINER
MAINTAINER sxlehua "sxlehua@qq.com"

# 修改来源
RUN sed -i 's/dl-cdn.alpinelinux.org/mirrors.aliyun.com/g' /etc/apk/repositories

# 修改时区
# RUN apk update \
# && apk add --no-cache bash tzdata \
# && ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime \
# && echo "Asia/Shanghai" > /etc/timezone

# 修改时区
RUN apk update \
&& apk add --no-cache bash tzdata \
&& cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime \
&& echo "Asia/Shanghai" > /etc/timezone \
&& apk del tzdata
