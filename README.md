# linuxcnc-dev

###### A docker image to run linuxcnc.

### Build it
```
./build.sh # you need to be in the directory of the repository
```

### Run it
if not already done you first need to do `xhost +` to allow docker to use your x-server.

```
docker run --rm -it -e DISPLAY=$DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix  linuxcnc-dev

```
