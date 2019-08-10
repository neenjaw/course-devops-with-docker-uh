# Ex 1.5

## Dockerfile

```dockerfile
FROM ubuntu:18.04

RUN apt-get update
RUN apt-get install -y curl
RUN apt-get install -y bash
```

## Commands

```sh
docker run -d -it --name curl-ex ubuntu:16.04 sh -c 'echo "Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website;'
docker exec -it curl-ex bash

#In the container
apt-get update
apt-get install curl
exit

#Outside the container
docker kill curl-ex
docker start -ai curl-ex
```
