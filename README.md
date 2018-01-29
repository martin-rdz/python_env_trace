

build the docker image

```
docker build -t python3-env .
```

run the image including a volumebinding
```
docker run -v /home/user/trace/:/trace -it python3-env /bin/bash
```
or with forwarding a port
```
docker run -v /home/user/trace/:/trace -p 8888:8888 -it python3-run /bin/bash
```


```
jupyter notebook --no-browser --ip=0.0.0.0
```
