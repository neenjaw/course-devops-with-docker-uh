# Ex 1.7

## Dockerfile

```dockerfile
FROM ubuntu:18.04

RUN apt-get update
RUN apt-get install -y curl
RUN apt-get install -y bash

ADD get_site.sh /

RUN chmod +x /get_site.sh

CMD /get_site.sh
```

## shell script

```bash
#!/bin/bash

echo "Input website:";

read website;

echo "Searching..";

sleep 1;

curl "http://${website}";
```
