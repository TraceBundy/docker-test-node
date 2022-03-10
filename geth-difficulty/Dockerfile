FROM registry.cn-hangzhou.aliyuncs.com/pressure/docker:go-ethereum-single-exe

ARG ACCOUNT_PASSWORD

COPY genesis.json /tmp

RUN geth init /tmp/genesis.json \
    && rm -f ~/.ethereum/geth/nodekey \

ENTRYPOINT ["geth"]
