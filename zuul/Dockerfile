#
# Dockerfile for Service C
#
FROM centos:centos7

FROM java:8

MAINTAINER Oreste Luci

# Install netcat
RUN yum update && yum install -y netcat

ADD target/zuul.jar zuul.jar

RUN bash -c 'touch /zuul.jar'

CMD ["/usr/lib/jvm/java-8-openjdk-amd64/bin/java", "-jar", "zuul.jar"]
