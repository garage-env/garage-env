# -------------------------------------------------------------------
# $ echo 'puts "Hello"' > hello.rb
# $ docker run -v `pwd`:/garage -t garage/ruby20 heloo.rb
# Hello
# -------------------------------------------------------------------

FROM garage/ruby20-base

MAINTAINER Reinaldo Junior <juniorz@gmail.com>

USER garage

CMD ["--help"]
ENTRYPOINT ["/usr/bin/ruby"]