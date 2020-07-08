FROM centos:7
RUN yum install -y wget net-tools git 
RUN wget https://github.com/prometheus/prometheus/releases/download/v2.18.1/prometheus-2.18.1.linux-amd64.tar.gz
RUN tar -xzf prometheus-2.18.1.linux-amd64.tar.gz
RUN mkdir prom_data
RUN cp -rvf prometheus-2.18.1.linux-amd64/* /
ENTRYPOINT [ "./prometheus" ]
CMD [ "--storage.tsdb.path='prom_data'" ]
EXPOSE 9090


