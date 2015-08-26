FROM ubuntu:14.04

RUN apt-get update && \
apt-get install -y curl openjdk-7-jre-headless

RUN curl -fL https://download.elastic.co/kibana/kibana/kibana-4.1.1-linux-x64.tar.gz | tar xzf - -C /opt && \
mv /opt/kibana-4.1.1-linux-x64 /opt/kibana

ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/kibana/bin

CMD ["kibana"]

EXPOSE 5601
