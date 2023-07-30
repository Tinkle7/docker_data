# create and run
```sh
docker run <image name>
```
- if the image is not there it will get the image from the hub
- create a container from the image
- start the container
> __Warning__
> Run for a short time then it will close. 

# default command override
```sh
## Run the container with the alternative command
docker run <image name> command
```
### example
```sh
## ls gives you all the files in the container.
docker run busybox ls 

## echo hi gives hi in the terminal.
docker run busybox echo hi 

## ping google.com help to run program infinite
docker run busybox ping google.com
```
```diff
+  run for long time `Cntrl + C` to stop
```
> __Warning__
> ls and echo are two programs inside the busybox file system if it's not it throws you an error.

# docker ps
```sh
## List all running containers
docker ps
## List all running containers that ever run in my machine.
docker ps --all
```
> __Note__
> docker ps help to get the id of all containers.


## container lifecycle
```diff 
+ docker run = ducker create + ducker start
```
```sh
## Create a container
docker create <image name>

## start a container
docker start <container id>
```
> __Note__
>`docker start` not gonna show you information coming out from the terminal, but `docker run` show you information coming out from the terminal.

```sh
## Start a container with logs
docker start -a <container id>
```
<sub>"-a" watch for output from the container and give it to your terminal.</sub>
