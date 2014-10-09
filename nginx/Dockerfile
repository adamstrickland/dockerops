FROM adamstrickland/base
MAINTAINER Adam Strickland <adam.strickland@gmail.com>

RUN apt-get install -y \
    dialog \
    net-tools \
    wget \
    nginx

RUN rm -v /etc/nginx/nginx.conf
ADD . /data
RUN ln -s /data/nginx.conf /etc/nginx/nginx.conf

EXPOSE 80
CMD service nginx start
