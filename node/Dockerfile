FROM jenkins/jenkins:lts

LABEL version="1.1" maintainer="colinchang<zhangcheng5468@gmail.com>"

ENV NODE_VERSION=14

USER root

# install node
RUN curl -sL https://deb.nodesource.com/setup_$NODE_VERSION.x | bash - \
&& apt update \
&& apt install -y nodejs \

# add jenkins to sudo
&& apt install -y sudo \
&& rm -rf /var/lib/apt/lists/* \
&& echo "jenkins ALL=NOPASSWD: ALL" >> /etc/sudoers \
&& apt clean

USER jenkins