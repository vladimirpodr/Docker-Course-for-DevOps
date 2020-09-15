FROM ubuntu:latest

ENV TZ=Europe/Kiev
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
RUN apt-get update
RUN apt-get install -y apt-utils
RUN apt-get install -y apache2
CMD /usr/sbin/apache2ctl -D FOREGROUND
EXPOSE 80