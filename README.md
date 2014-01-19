## docker-cgminer-hex

A Docker for transforming your Raspberry Pi into a controller for HEX Bitcoin miners.

### Preparing your Raspberry Pi

In order to get [Docker](https://www.docker.io/) up and running on your Raspberry Pi, I suggest you follow the instructions in this [blog posting](http://resin.io/blog/docker-on-raspberry-pi-in-4-simple-steps/). It's really simple.

### Running cgminer

```bash
root@alarmpi ~ docker run -t -i -privileged -v /dev/bus/usb:/dev/bus/usb b00gizm/rpi-cgminer-hex /usr/local/bin/cgminer
```

or, if you prefer CLI arguments:

```bash
root@alarmpi ~ docker run -t -i -privileged -v /dev/bus/usb:/dev/bus/usb b00gizm/rpi-cgminer-hex /usr/local/bin/cgminer -o <server> -u <username> -p <password>
```

### Author

Pascal Cremer ([@b00gizm](http://twitter.com/b00gizm))
