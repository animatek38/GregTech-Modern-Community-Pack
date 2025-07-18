# syntax=docker/dockerfile:1

FROM openjdk:17-buster

RUN apt-get update && apt-get install -y curl unzip


USER minecraft

COPY start.sh /start.sh
RUN chmod +x /start.sh

VOLUME /data
WORKDIR /data

EXPOSE 25565/tcp

CMD ["/start.sh"]
