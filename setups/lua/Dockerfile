FROM garage/base

MAINTAINER Reinaldo Junior <juniorz@gmail.com>

RUN apt-get update && apt-get upgrade -y

RUN /var/garage/install lua5.1

# Clean up APT when done.
RUN apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

ENV GARAGE_PROVIDES lua luac