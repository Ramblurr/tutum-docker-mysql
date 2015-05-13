FROM ubuntu:trusty
MAINTAINER Casey Link <casey@outskirtslabs.com>

WORKDIR /

# Expose environment variables
ENV MYSQL_PASS **ChangeMe**
ENV MYSQL_USER **ChangeMe**

RUN apt-get update && \
    mkdir -p /var/lib/mysql && \
    mkdir -p /etc/mysql && \
    apt-get -yq install mysql-client

VOLUME  ["/etc/mysql", "/var/lib/mysql"]

ENTRYPOINT /usr/bin/tail -f /dev/null
