ARG ELK_VERSION

# https://github.com/elastic/logstash-docker
FROM docker.elastic.co/logstash/logstash:${ELK_VERSION}

ADD mysql-connector-java-8.0.13.jar /usr/share/logstash/logstash-core/lib/jars/mysql-connector-java-8.0.13.jar

RUN logstash-plugin install logstash-input-jdbc
# Add your logstash plugins setup here
# Example: RUN logstash-plugin install logstash-filter-json
