FROM docker.elastic.co/logstash/logstash:7.3.2
# копируем из текущей директории файл конфигурации в контейнер
COPY logstash.conf /usr/share/logstash/pipeline
# копируем из текущей директории файл конфигурации в контейнер
COPY logstash.yml /usr/share/logstash/config
ENV TZ=Europe/Moscow
