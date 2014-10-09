FROM ubuntu:trusty
MAINTAINER Adam Strickland <adam.strickland@gmail.com>

RUN apt-get update

# install dependencies
RUN apt-get install -y build-essential \
                       autoconf \
                       imagemagick \
                       libevent-dev \
                       libffi-dev \
                       libglib2.0-dev \
                       libjpeg-dev \
                       libmagickcore-dev \
                       libmagickwand-dev \
                       libncurses-dev \
                       zlib1g-dev \
                       libssl-dev \
                       libreadline6-dev \
                       libyaml-dev \
                       libxml2-dev \
                       libxslt1-dev \
                       libcurl4-openssl-dev \
                       software-properties-common

# tools
RUN apt-get install -y git \
                       vim \
                       tmux \
                       curl
