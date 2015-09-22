# This is a Dockerfile to build a opensuse image which run mariadb
FROM ubuntu:14.04
MAINTAINER Mengz You <mengz.you@outlook.com>

# Environments
ENV OS_NAME "Ubuntu"
ENV OS_VERSION_ID "14.04"
ENV OS_VERSION "14.04.3 LTS, Trusty Tahr"

# Update and install tool packages
RUN apt-get update \
  && apt-get install -y curl \
  && apt-get clean

# Change the timezone to PRC
RUN rm /etc/localtime \
  && ln -s /usr/share/zoneinfo/Asia/Chongqing /etc/localtime
