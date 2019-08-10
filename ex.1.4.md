# Ex 1.4

## Commands

```sh
docker run -d --rm --name bash-ex devopsdockeruh/exec_bash_exercise
docker exec -it bash-ex bash

#In the container
tail -f ./logs.txt

Secret message is:
"Docker is easy"
```
