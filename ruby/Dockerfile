FROM adamstrickland/base
MAINTAINER Adam Strickland <adam.strickland@gmail.com>

# install ruby 2.1.2
RUN curl http://ftp.ruby-lang.org/pub/ruby/2.1/ruby-2.1.2.tar.gz > /tmp/ruby-2.1.2.tar.gz
WORKDIR /tmp
RUN tar -xvzf ruby-2.1.2.tar.gz
WORKDIR /tmp/ruby-2.1.2
RUN ./configure --prefix=/usr/local
RUN make
RUN make install

# install rubygems
RUN curl http://production.cf.rubygems.org/rubygems/rubygems-2.4.1.tgz > /tmp/rubygems-2.4.1.tgz
WORKDIR /tmp
RUN tar -xzvf rubygems-2.4.1.tgz
WORKDIR /tmp/rubygems-2.4.1
RUN ruby setup.rb
RUN echo "gem: --no-ri --no-rdoc" >> /usr/local/etc/gemrc

# install some helper gems
RUN gem install bundler foreman

WORKDIR /
