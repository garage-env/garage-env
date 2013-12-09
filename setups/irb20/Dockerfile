# -------------------------------------------------------------------
# $ docker run -i -v `pwd`:/garage -t garage/irb20
# -------------------------------------------------------------------

FROM garage/ruby20-base

MAINTAINER Reinaldo Junior <juniorz@gmail.com>

USER garage

CMD ["-I", "/garage"]
ENTRYPOINT ["/usr/bin/irb"]