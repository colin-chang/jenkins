FROM jenkins/jenkins:lts-centos

LABEL version="1.0" maintainer="colinchang<zhangcheng5468@gmail.com>"

ENV DOTNET_VERSION=5.0
ENV NODE_VERSION=14

USER root

# dotnet 
RUN dnf install -y dotnet-sdk-$DOTNET_VERSION \

# node
&& dnf install -y gcc-c++ make \
&& curl -sL https://rpm.nodesource.com/setup_$NODE_VERSION.x | bash - \
&& dnf install -y nodejs

USER jenkins