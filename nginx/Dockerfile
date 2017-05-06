FROM nginx

ARG BASIC_USER
ARG BASIC_PASS

RUN apt-get update \
    && apt-get install -y apache2-utils \
    && htpasswd -bc /etc/nginx/.htpasswd ${BASIC_USER} ${BASIC_PASS} \
    && apt-get remove -y apache2-utils \
    && rm -rf /var/lib/apt/lists/*


ADD ./conf.d/default.conf /etc/nginx/conf.d/default.conf
