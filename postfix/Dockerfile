FROM ubuntu:12.10

RUN apt-get update
RUN apt-get -y upgrade

RUN apt-get install -y postfix
RUN apt-get install -y dovecot-common  dovecot-imapd 
RUN apt-get install -y supervisor

ADD ./supervisord.conf /etc/supervisor/supervisord.conf
ADD ./main.cf /etc/postfix/main.cf

EXPOSE 25 25

#CMD ["/usr/bin/supervisord"]
ENTRYPOINT ["/usr/bin/supervisord"]
