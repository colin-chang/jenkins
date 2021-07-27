FROM jenkins/jenkins:lts-centos

LABEL version="1.0" maintainer="colinchang<zhangcheng5468@gmail.com>"

ENV NODE_VERSION=14

USER root

# node
RUN dnf install -y gcc-c++ make \
&& curl -sL https://rpm.nodesource.com/setup_$NODE_VERSION.x | bash - \
&& dnf install -y nodejs \

# vuepress
&& npm install -g yarn \
&& yarn add -D vuepress

USER jenkins