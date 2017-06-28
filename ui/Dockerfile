FROM storm-base
ENV NIMBUS nimbus
ENV ZOOKEEPER zookeeper
WORKDIR /var/opt/apache-storm-1.1.0
CMD ["sh", "-c", "./bin/storm ui -c nimbus.seeds=[\\\"${NIMBUS}\\\"] -c storm.zookeeper.servers=[\\\"$ZOOKEEPER\\\"]"]
