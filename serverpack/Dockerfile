# syntax=docker/dockerfile:1
#Original file from https://github.com/Goobaroo/docker-allthemods9/blob/main/Dockerfile
FROM openjdk:17-buster

RUN apt-get update && apt-get install -y curl unzip

COPY start.sh /start.sh
RUN chmod +x /start.sh

VOLUME /data
WORKDIR /data

EXPOSE 25565/tcp

CMD ["/start.sh"]
