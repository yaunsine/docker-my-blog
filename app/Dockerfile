FROM openjdk:8-jdk-alpine
MAINTAINER "维护者 <email>"
LABEL description="blog imagec"
WORKDIR app
# RUN apt-get update && apt-get install -y fontconfig

RUN set -xe \
&& apk --no-cache add fontconfig
#&& apk --no-cache add ttf-dejavu fontconfig
COPY msyh.ttc /usr/share/fonts/ttf-dejavu/simsun.ttc
ADD my-blog-4.0.0-SNAPSHOT.jar /app/app.jar
EXPOSE 8081
CMD java -jar /app/app.jar
