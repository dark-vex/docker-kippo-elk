# https://github.com/elastic/logstash-docker
FROM docker.elastic.co/logstash/logstash-oss:6.1.0

# Add your logstash plugins setup here
# Example: RUN logstash-plugin install logstash-filter-json
USER root
RUN yum install -y wget gzip && wget "http://geolite.maxmind.com/download/geoip/database/GeoLiteCity.dat.gz" && wget "http://download.maxmind.com/download/geoip/database/asnum/GeoIPASNum.dat.gz" && gunzip *.dat.gz 
