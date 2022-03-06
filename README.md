# Docker Command



## Start Docker Engine
```
service docker start
```



## Check Docker Version and Info
```
docker version
```
```
docker info
```
## Check container exits or not
```
docker container ls
```



## Check Image exits or not
```
docker image ls
```



## Check Network
```
docker network ls
```



## Show running Container
```
docker ps
```



## Container run from Image
```
docker container run ubuntu
```




## Container Remove
```
docker container rm 191c1
```



## Docker Container Start
```
docker container start 191c1
```



## Docker Container Stop
```
docker container stop 191c1
```



## When create container and run background
```
docker container run -d ubuntu
```




## When create container and run background and login container
```
docker container run -d -it ubuntu /bin/bash
```




## When c
```
apt-get
```



## How to exit from container and container stop
Ctrl + d, or type exit



## How to exit from container but container not stop
Ctrl + pq




## How to remove all container in one command
```
docker container rm $(docker container ls -aq)
```







## How to show how and what process running in docker container
```
docker container top dl891
```



## container and run port
```
docker container run -d -p 3600:80 –name test_web nginx
```



## How to check what port is open
```
Netstat -nltp
```



## How to check container ip address
```
docker container inspect 615
```



## How to login into container
```
docker container exec –it 65434 /bin/bash
```

## How to change container tagname
```
docker container rename 2343432 tiger_web
```




## How to restart container
```
docker container restart 2343432
```



## Attach command use for background process to foreground container
```
docker container attach 58
```






## docker container Kill
```
docker container kill 58
```



## docker container Paused
```
docker container pause 58
```



## docker container UnPaused
```
docker container unpause 58
```



## How to check container port
```
docker container port 122323
```





## how to export
```
docker container export 23423423 > my_ubuntu_tree_git.tar
```




## how to Import
```
docker image import my_ubuntu_tree_git.tar my_ubuntu_t_g
```




Video 12
=================
At first make container and make some file in container



## How to make Image from container
```
docker container commit –author “Md Mehrab Hossain” -m “this is test commit” 234324234 newImage_name
```




Video 13
=================
## How to login docker
```
docker login
```




## How to pull image
```
docker pull ubuntu:14.04 //last a version name , version na dile o kaj korbe
```



## Image Tag
```
docker image tag my_ubuntu_t_g mahabub01/my_ubuntu_tree_git
// my_ubuntu_t_g ata hossa old tag name
// image push korte hole docker hub ar username diye image tag korte hobe
```



## How to image push
```
docker push mahabub01/my_ubuntu_tree_git
```



Video 14
========
## docker Image Command
```
docker image ls



Docker image ls –format ‘{{.ID}} , {{.Repository}} - {{.Tag}}’



```



## How to show image history
```
docker image history jenkins
```



## How to remove image
```
docker image rm -f mahabub01/my_ubuntu_tree_git
```
## How to show image required configure
```
docker image inspect mahabub01/my_ubuntu_tree_git |less
```




Video 15
==============
## How to docker image save tar file
```
docker image save mahabub01/my_ubuntu_tree_git |less > myimage.tar
```



## How load docker image tar file
```
docker image load < myimage.tar
```
Note:
=> Docker image save
=> docker container export
2ta command e tar file generate kore ….. Tobe save korar time a a jodi version ullekh na kora hoi tahole oi image ar joto version ache all version tar file generate kore dibe




## Environment variables are supported by the following list of instructions in the Dockerfile:
```
ADD
COPY
ENV
EXPOSE
FROM
LABEL
STOPSIGNAL
USER
VOLUME
WORKDIR
ONBUILD (when combined with one of the supported instructions above)
```
