##Spark镜像说明文档
###环境
* ubuntu14.04 64bit
* jre_1.8

###基础镜像
基础镜像是自己根据Docker官方的Ubuntu：14.04为基础镜像升级而来，主要有以下改进
1. 修改软件源为aliyun软件源
2. apt-get update && apt-get -y upgrade && apt-get install -y vim
3. 基本的vim配置
4. 基础镜像配置：`ubuntu:14.04 64bit`

这个基础镜像的Dockerfile见[我的github地址](https://github.com/adolphlwq/DockerfileHub)

###Spark镜像
#####软件环境
* 安装jre并配置环境变量

#####功能
* 基础java环境

