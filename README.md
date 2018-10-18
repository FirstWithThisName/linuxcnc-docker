# linuxcnc-docker

###### A docker image to run linuxcnc.

### Build it

##### Requirements for the build:
* run docker as current user
* installed git

```
./build.sh # you need to be in the directory of the repository
```

### Get the binary image
```
docker pull aceofdiamonds/linuxcnc-docker
```

### Run it
if not already done you first need to do `xhost +` to allow docker to use your x-server.

```
docker run --rm -it -e DISPLAY=$DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix  linuxcnc-dev

```
