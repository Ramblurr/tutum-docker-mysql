FROM ubuntu:trusty
MAINTAINER Casey Link <casey@outskirtslabs.com>

WORKDIR /

# Expose environment variables
ENV MYSQL_PASS **ChangeMe**
ENV MYSQL_USER **ChangeMe**

RUN mkdir -p /var/lib/mysql
VOLUME  ["/var/lib/mysql"]

ENTRYPOINT /usr/bin/tail -f /dev/null
