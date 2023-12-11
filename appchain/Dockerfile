FROM registry.cn-hangzhou.aliyuncs.com/pressure/docker:platon-single-exe

ADD data /appchain/data
COPY genesis.json /appchain/data

RUN platon init /appchain/data/genesis.json --datadir /appchain/data/

ENTRYPOINT ["platon"]
