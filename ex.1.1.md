# Ex 1.1

## Commands

```console
docker run -d --name ng-container nginx
docker run -d --name pg-container postgres
docker run -d --name rd-container redis

docker stop ng-container
docker stop pg-container

docker ps

docker stop rd-container

docker containers purge
docker images purge
```
