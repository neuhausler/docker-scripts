FROM marcel/precise-20131128
MAINTAINER Marcel Neuhausler

RUN apt-get install -y git-core
RUN apt-get install -y wget unzip

RUN apt-get install -y openjdk-6-jdk
ENV JAVA_HOME /usr/lib/jvm/java-6-openjdk-amd64/

RUN apt-get install -y build-essential libncurses5-dev openssl libssl-dev fop xsltproc unixodbc-dev
RUN mkdir -p /tmp/erlang
RUN cd /tmp/erlang && wget http://erlang.org/download/otp_src_R15B03.tar.gz
RUN cd /tmp/erlang && tar zxvf otp_src_R15B03.tar.gz
RUN cd /tmp/erlang/otp_src_R15B03 && ./configure && make && sudo make install


 