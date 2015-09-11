#base java env

FROM adolphlwq/ubuntu:base_14.04
MAINTAINER adolphlwq <kenan3015@gmail.com>

ENV REFRESHED_AT 2015-9-11

#install wget
RUN apt-get install -yqq wget

#install java
RUN cd /opt && wget --no-cookies --no-check-certificate --header "Cookie: oraclelicense=accept-securebackup-cookie" \
				"http://download.oracle.com/otn-pub/java/jdk/8u45-b14/jdk-8u45-linux-x64.tar.gz" && \
				tar -xvf jdk-8u45-linux-x64.tar.gz && rm jdk-8u45-linux-x64.tar.gz

ADD env_config  /opt/
RUN cat /opt/env_config >> /etc/bash.bashrc && rm /opt/env_config

CMD ["bin/bash","java -v"] 
