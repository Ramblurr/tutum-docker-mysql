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

VOLUME  ["/var/lib/mysql"]

ADD my.cnf.minimal /etc/mysql/my.cnf
ADD mysqld_charset.cnf /etc/mysql/conf.d/mysqld_charset.cnf

ENTRYPOINT /usr/bin/tail -f /dev/null
