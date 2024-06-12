# 使用Python3基础镜像
FROM python:3.10-alpine

# 安装基础依赖
RUN apk add gcc g++ make libffi-dev openssl-dev libtool wget

# 下载Nodejs源码，并解压归档文件
RUN cd /home && wget https://nodejs.org/dist/v18.20.0/node-v18.20.0.tar.gz && tar zxvf node-v18.20.0.tar.gz

# 编译Nodejs
RUN cd /home/node-v18.20.0 && ./configure && make && make install
