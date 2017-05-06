FROM jenkins

USER root
RUN apt-get update \
    && apt-get install -y maven

RUN wget https://storage.googleapis.com/golang/go1.8.1.linux-amd64.tar.gz -P /tmp \
    && tar -C /usr/local -xzf /tmp/go1.6.linux-amd64.tar.gz \
    && export PATH=$PATH:/usr/local/go/bin \
    && echo 'export PATH=$PATH:/usr/local/go/bin' >> /etc/bashrc
