# linuxcnc-dev

A docker image to run linuxcnc for testing.

### Build it
`docker build -t linuxcnc-dev`

### Run it
if not allready done you first need to do `xhost +` to allow docker to use your x-server.

```
docker run --rm -it -e DISPLAY=$DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix  linuxcnc-dev

```
