# Hyperledger Project 

### Software Information

| Software    | Version            |
|-------------|--------------------|
| Vagrant     | 2.2.4              |
| Vagrant Box | bento/ubuntu-18.04 |
| VirtualBox  | 6.0                |
| OS          | Ubuntu 18.04.1 LTS |

### Installation

```
$ git clone git@github.com:eitake0002/hyperledger-fabric.git
$ cd hyperledger-fabric
$ vagrant up

# Login to vagrant
$ vagrant ssh
```

### Hyperledger Composer

Hyperledger Composer is a development framework to build blockchain application with ease. Currently, Hyperledger Composer supports only Hyperledger Fabric infrastructure and runtime. 

https://hyperledger.github.io/composer/latest/introduction/introduction.html

# Sawtooth

Open source code for sawtooth PoC project. 

### Prerequisite

Install docker engine, and compose. 

### Commands

```
# Docker compose up. sawtooth default docker compose.
$ docker-compose -f sawtooth-default.yaml up

# Down docker compose.
$ docker-compose -f sawtooth-default.yaml down

# Check docker container.
$ docker ps

# Login to docker shell.
$ docker exec -it sawtooth-shell-default bash

# Check blocks.
$ curl http://localhost:8008/blocks
```
