# dockerfiles-ubuntu-user-adderable
Ubuntu, It support base user creation and password setting.

# Building & Running

Copy the sources to your docker host and build the container, and to run.
```
	docker build -t woogi43/ubuntu:test .
	docker run -it --name u1  woogi43/ubuntu:test
```
Get the port that the container is listening on:

```
# docker ps
CONTAINER ID        IMAGE                COMMAND             CREATED             STATUS              PORTS               NAMES
fc199e02d300        nowage/ubuntu:test   "/bin/bash"         41 seconds ago      Up 40 seconds                           u1
```


To Rollback
```
    docker rm u1 -f
    docker rmi woogi43/ubuntu:test
```
