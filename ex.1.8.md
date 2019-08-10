# Ex 1.8

```sh
mkdir app
touch app/logs.txt
docker run -v $(pwd)/app/logs.txt:/usr/app/logs.txt devopsdockeruh/first_volume_exercise
```
