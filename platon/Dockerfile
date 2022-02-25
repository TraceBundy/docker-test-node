FROM registry.cn-hangzhou.aliyuncs.com/pressure/docker:platon-single-exe

ADD data /tmp/data
COPY genesis.json /tmp/data

RUN platon init /tmp/data/genesis.json --datadir /tmp/data/

ENTRYPOINT ["platon"]
