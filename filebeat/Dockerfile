FROM docker.elastic.co/beats/filebeat:8.9.1
COPY filebeat.yml /etc/filebeat/filebeat.yml:ro
COPY cisco.yml /etc/filebeat/modules.d/cisco.yml
USER root
RUN apt-get install curl
RUN filebeat modules enable cisco