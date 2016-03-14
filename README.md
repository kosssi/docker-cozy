# Docker for Cozy

## Create development environment

Create docker machine:

    docker-machine create --driver virtualbox cozy.dev

Link docker machine:

    eval $(docker-machine env cozy.dev)

Get all docker images

