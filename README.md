# Docker-storm

Docker storm is a docker-compose file including Dockerfiles for openJDK and oracleJDK. In order to use the oracleJDK image you have to login to Dockerhub and get the image from the Docker store. Change the "volume:" in the docker-compose.yaml according to your topology target folder.

### Usage

```sh
$ docker-compose up
```
The Storm ui will be available on http://localhsot:8080. To deploy a topology run the following according to your target directory
```sh
$ run --rm  storm-base ./bin/storm jar -c nimbus.host=nimbus /var/opt/mytopologies/storm-starter-1.1.0.jar org.apache.storm.starter.WordCountTopology WordCount
```

