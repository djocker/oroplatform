# OROPlatform Docker Image
[![GitHub tag](https://img.shields.io/github/tag/djocker/oroplatform.svg?maxAge=2592000)](https://hub.docker.com/r/djocker/oroplatform/tags/) [![Docker Pulls](https://img.shields.io/docker/pulls/djocker/oroplatform.svg?maxAge=2592000)](https://hub.docker.com/r/djocker/oroplatform/)  

The docker image contains source code of OROPlatform application.
This image are used as part of docker stack (see compose configs).

## Requirements

1. [Docker](https://www.docker.com/)
2. [Docker Compose](http://docs.docker.com/compose)

## Usage
**OROPlatform stack with web installation**

For more information [see compose config](./compose/webinstall/docker-compose.yml)

Run stack 

```
docker-compose -f <(curl https://raw.githubusercontent.com/djocker/oroplatform/master/compose/webinstall/docker-compose.yml) up
```
Navigate to [http://localhost:3080](http://localhost:3080) in your web browser, and install application via web wizard

Stop stack

```
docker-compose -f <(curl https://raw.githubusercontent.com/djocker/oroplatform/master/compose/webinstall/docker-compose.yml) stop
```

**OROPlatform stack with automated installation**

For more information [see compose config](./compose/autoinstall/docker-compose.yml)

default login: `admin` default password: `admin1111`

Run stack
```
docker-compose -f <(curl https://raw.githubusercontent.com/djocker/oroplatform/master/compose/autoinstall/docker-compose.yml) up
```
Navigate to [http://localhost:3080](http://localhost:3080) in your web browser, and login

Stop stack
```
docker-compose -f <(curl https://raw.githubusercontent.com/djocker/oroplatform/master/compose/autoinstall/docker-compose.yml) stop 
```
