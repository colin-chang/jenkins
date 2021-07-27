FROM jenkins/jenkins:lts-centos

LABEL version="1.0" maintainer="colinchang<zhangcheng5468@gmail.com>"

ENV DOTNET_VERSION=5.0

USER root

# dotnet 
RUN dnf install -y dotnet-sdk-$DOTNET_VERSION

USER jenkins