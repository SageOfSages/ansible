# скачиваю образ с сайта эластик
FROM docker.elastic.co/beats/filebeat:7.3.2
# копируем из текущей директории файл конфигурации в контейнер
COPY filebeat.yml /usr/share/filebeat
# позволяет делать изменения в контейнере от пользователя рут
USER root
# скопированному файлу изменяем набор прав в самом контейнере
RUN cd /usr/share/filebeat && chmod go-w /usr/share/filebeat/filebeat.yml
#  тайм зона
ENV TZ=Europe/Moscow