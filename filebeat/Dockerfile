FROM docker.elastic.co/beats/filebeat:6.6.1
COPY filebeat.yml /usr/share/filebeat
USER root
RUN mkdir /usr/share/filebeat/nginx
RUN chmod 775 /usr/share/filebeat/nginx
RUN chown filebeat /usr/share/filebeat/filebeat.yml && chmod go-w /usr/share/filebeat/filebeat.yml

RUN ls
USER filebeat