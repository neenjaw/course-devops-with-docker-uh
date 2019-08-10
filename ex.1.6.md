# Ex 1.6

## Dockerfile

```dockerfile
FROM devopsdockeruh/overwrite_cmd_exercise

ENTRYPOINT ["./start.sh", "-c", "1"]
```

## Commands

```sh
# Overrides entry point to get a shell in the container
docker run -it --entrypoint sh docker-clock

# Tags the build from the dockerfile, tag it `docker-clock`
docker build -t docker-clock .

# run container interactively
docker run -it docker-clock
```
