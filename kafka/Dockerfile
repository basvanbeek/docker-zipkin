FROM quay.io/openzipkin/zipkin-base:base-1.39.4
MAINTAINER OpenZipkin "http://zipkin.io/"

ENV SCALA_VERSION 2.11
ENV KAFKA_VERSION 0.9.0.0
ENV ZOOKEEPER_VERSION 3.4.6

WORKDIR /kafka
ADD install.sh /kafka/install
RUN /kafka/install

EXPOSE 2181 9092

CMD ["runsvdir", "/etc/service"]
