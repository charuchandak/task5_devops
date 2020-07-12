FROM centos:7
RUN yum -y install net-tools wget
RUN wget https://dl.grafana.com/oss/release/grafana-7.0.3-1.x86_64.rpm

RUN yum -y install grafana-7.0.3-1.x86_64.rpm
WORKDIR /usr/share/grafana
EXPOSE 3000
CMD /usr/sbin/grafana-server start && /usr/sbin/grafana-server enable && /bin/bash


