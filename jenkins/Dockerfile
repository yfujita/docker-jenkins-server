FROM jenkins

USER root
RUN apt-get update \
    && apt-get install -y maven \
    && add-apt-repository ppa:ubuntu-lxc/lxd-stable \
    && apt-get update \
    && apt-get install -y golang
