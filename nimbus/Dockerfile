FROM storm-base
ENV ZOOKEEPER zookeeper
WORKDIR /var/opt/apache-storm-1.1.0
CMD ["sh", "-c", "./bin/storm nimbus -c storm.zookeeper.servers=[\\\"$ZOOKEEPER\\\"]"]
