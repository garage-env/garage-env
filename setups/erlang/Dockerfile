FROM garage/base

MAINTAINER Reinaldo Junior <juniorz@gmail.com>

RUN apt-get update && apt-get upgrade -y

## Installs Erlang from Erlang Solutions
RUN /var/garage/install curl &&\
    curl -q http://packages.erlang-solutions.com/debian/erlang_solutions.asc | apt-key add - &&\
    echo 'deb http://packages.erlang-solutions.com/debian saucy contrib' > /etc/apt/sources.list.d/erlang-solutions.list &&\
    apt-get update &&\
    /var/garage/install erlang

# Clean up APT when done.
RUN apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

# Provides erl and erlc
ENV GARAGE_PROVIDES erl erlc