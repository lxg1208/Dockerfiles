FROM lxg1208/jdk:1.7
MAINTAINER lxg1208 (xuegang_1208@163.com)

ADD tomcat7.tar.gz /opt/
COPY supervisord.conf /etc/supervisord.conf

ENV CATALINA_HOME /opt/tomcat7

VOLUME [${CATALINA_HOME}"/webapps/"]

EXPOSE 8080

CMD ["/usr/bin/supervisord"]