FROM adamstrickland/ruby
MAINTAINER Adam Strickland <adam.strickland@gmail.com>

# install some other stuff
RUN apt-get install -y bison \
                       procps \
                       nodejs

EXPOSE 3000
CMD bundle install --system --without test developement && PORT=3000 foreman start

#
# sample usage:
#
# FROM adamstrickland/rails
#
# RUN apt-get install -y libsqlite3-dev sqlite3
#
# WORKDIR /tmp
# ADD ./Gemfile Gemfile
# ADD ./Gemfile.lock Gemfile.lock
# RUN bundle install
#
# ADD . /var/application
# WORKDIR /var/application
#
# CMD PORT=3000 foreman start
