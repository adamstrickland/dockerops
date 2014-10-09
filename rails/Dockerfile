FROM adamstrickland/ruby
MAINTAINER Adam Strickland <adam.strickland@gmail.com>

# install some other stuff
RUN apt-get install -y bison \
                       procps \
                       nodejs

EXPOSE 3000
CMD bundle install --system --without test developement && PORT=3000 foreman start

# ADD . /var/application
# WORKDIR /var/application
