#base iamge using aliyun source lists

FROM ubuntu:14.04
MAINTAINER SuJianchao <sujianchao@gmail.com>

#backup old sources.list
RUN cd /etc/apt/ && mv sources.list sources.lists_backup

#add new sources.list
ADD sources.list /etc/apt/

#upgrade
RUN apt-get update && apt-get upgrade -y

LABEL sources="mirrors.163.com"

CMD ["/bin/bash"]
