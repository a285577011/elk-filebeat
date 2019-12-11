ARG ELK_VERSION

# https://github.com/elastic/logstash-docker
FROM docker.elastic.co/logstash/logstash:${ELK_VERSION}
RUN logstash-plugin install logstash-input-jdbc
#安装output插件
RUN logstash-plugin install logstash-output-elasticsearch
# Add your logstash plugins setup here
# Example: RUN logstash-plugin install logstash-filter-json
#容器启动时执行的命令.(CMD 能够被 docker run 后面跟的命令行参数替换)
