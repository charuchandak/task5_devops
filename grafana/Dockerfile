FROM centos:7
RUN yum -y install net-tools wget
RUN wget https://dl.grafana.com/oss/release/grafana-7.0.3-1.x86_64.rpm

RUN yum -y install grafana-7.0.3-1.x86_64.rpm
WORKDIR /usr/sbin/grafana/

CMD [ "/usr/sbin/grafana-server", "cfg:default.paths.data=/var/lib/grafana", "config=/etc/grafana/grafana.ini" ]

EXPOSE 3000

