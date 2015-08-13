FROM quyennt/ubuntu
MAINTAINER quyen@agencyrevolution

RUN . /etc/lsb-release && echo "deb http://download.rethinkdb.com/apt $DISTRIB_CODENAME main" | sudo tee /etc/apt/sources.list.d/rethinkdb.list

RUN wget -qO- http://download.rethinkdb.com/apt/pubkey.gpg | sudo apt-key add -

RUN apt-get update

RUN apt-get install -y rethinkdb

VOLUME /data

WORKDIR /data
