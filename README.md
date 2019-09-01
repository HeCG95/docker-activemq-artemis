# docker-activemq-artemis 
**Activemq Artemis with Docker Compose** 

Using Docker Compose to create an activemq artemis.

## Prerequisite

+ Install [Docker][1] and [Docker Compose][2] in your testing environment

## Start with following steps

+ (1) Start activemq artemis

```
docker-compose up -d
```

The result is 

```
Creating docker-activemq-artemis_activemq-artemis_1 ... done   
```

+ (2) Check the status of activemq artemis

```
docker-compose ps
```

The result is 

```
                   Name                                 Command               State                                                  Ports                                               
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
docker-activemq-artemis_activemq-artemis_1   /docker-entrypoint.sh arte ...   Up      1883/tcp, 5445/tcp, 5672/tcp, 61613/tcp, 0.0.0.0:61616->61616/tcp, 0.0.0.0:8161->8161/tcp, 9404/tcp
```

+ (3) View activemq management console on : http://hostname:8161/console/login, with username - artemis, with password - artemis.


[1]: https://www.docker.com
[2]: https://docs.docker.com/compose/

## License

Apache 2.0 license
