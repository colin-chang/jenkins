FROM jenkins/jenkins:lts

LABEL version="1.1" maintainer="colinchang<zhangcheng5468@gmail.com>"

ENV NODE_VERSION=14

USER root

# node
RUN curl -sL https://deb.nodesource.com/setup_$NODE_VERSION.x | bash - \
&& apt update \
&& apt install -y nodejs

USER jenkins