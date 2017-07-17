FROM alpine
MAINTAINER lxg1208 (xuegang_1208@163.com)

ENV TZ "Asia/Shanghai"
ENV LANG C.UTF-8

RUN echo "https://mirror.tuna.tsinghua.edu.cn/alpine/v3.6/main" > /etc/apk/repositories

RUN apk add --update \
    bash \
    python \
    py-pip \
    py-meld3 \
#    build-base \
    && rm -rf /var/cache/apk/*

ADD supervisor-3.3.2.tar.gz .
RUN cd supervisor-3.3.2 && python setup.py install

RUN apk --no-cache add ca-certificates
COPY sgerrand.rsa.pub /etc/apk/keys/sgerrand.rsa.pub
COPY glibc-2.25-r0.apk .
RUN apk add glibc-2.25-r0.apk

