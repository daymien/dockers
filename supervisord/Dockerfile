from ubuntu:12.04
maintainer Reimund Klain

run apt-get update
run apt-get -y upgrade
run apt-get install -y python-setuptools
run easy_install supervisor

#ENTRYPOINT ["/usr/local/bin/supervisord", "-n", "-c", "/etc/supervisord.conf"]
