#base jre env

FROM adolphlwq/ubuntu:base_14.04
MAINTAINER adolphlwq <kenan3015@gmail.com>

ENV REFRESHED_AT 2015-9-11

#install wget
RUN apt-get install -yqq wget

#install java
RUN cd /opt && wget --no-cookies --no-check-certificate --header "Cookie: oraclelicense=accept-securebackup-cookie" \
				"http://javadl.sun.com/webapps/download/AutoDL?BundleId=109700" && \
				tar -xvf jre-8u60-linux-x64.tar.gz && rm jre-8u60-linux-x64.tar.gz

ADD env_config  /opt/
RUN cat /opt/env_config >> /etc/bash.bashrc && rm /opt/env_config

CMD ["bin/bash"] 
