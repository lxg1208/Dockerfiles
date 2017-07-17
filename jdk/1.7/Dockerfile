FROM lxg1208/base
MAINTAINER lxg1208 (xuegang_1208@163.com)

ADD jdk1.7.tar.gz /usr/local/

ENV JAVA_HOME /usr/local/jdk1.7
ENV JRE_HOME $JAVA_HOME/jre
ENV CLASSPATH $JAVA_HOME/lib/dt.jar:$JAVA_HOME/lib/tools.jar:$JAVA_HOME/lib
ENV PATH $PATH:$JAVA_HOME/bin:$JRE_HOME/bin:
