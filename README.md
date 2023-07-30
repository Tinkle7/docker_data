# create and run
```sh
docker run <image name>
```
- if the image is not there it will get the image from the hub
- create a container from the image
- start the container
 > Run for a short time then it will close

# default command override
```sh
docker run <image name> command
```
### example
```sh
docker run busybox ls 
```
>ls gives you all the files in the container.
```sh
docker run busybox echo hi 
```
> echo hi gives hi in the terminal.
```sh
docker run busybox ping google.com
```
> run for long time `Cntrl + C` to stop`

```diff
@@ ls and echo are two programs inside the busybox file system if it's not it throws you an error.@@
```

# docker ps
```sh
docker ps
```
> List all running containers
```sh
docker ps --all
```
> List all running contatners that ever run in my machine.

```diff
@@ docker ps help to get id of all containers.@@
```
