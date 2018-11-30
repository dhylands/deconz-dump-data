This repository contains a sample capture of USB serial
data between the [deConz](https://www.dresden-elektronik.de/funktechnik/products/software/pc-software/deconz/?L=1)
program and the [ConBee](https://shop.dresden-elektronik.de/conbee.html) USB dongle.

The [deconz-zcl.json](https://raw.githubusercontent.com/dhylands/deconz-dump-data/master/deconz-zcl.json)
file was created from WireShark by following
the process outlined [here](http://blog.davehylands.com/capturing-usb-serial-using-wireshark/)

The [deconz-zcl.log](https://raw.githubusercontent.com/dhylands/deconz-dump-data/master/deconz-zcl.log)
file was produced by running the following:
```
git clone https://github.com/dhylands/deconz-dump-data
git clone https://github.com/mozilla-iot/deconz-api
cd deconz-api
npm install
cd dump
./dump.js ../../deconz-dump-data/deconz-zcl.json
```

The [deconz-zcl-detail.log](https://raw.githubusercontent.com/dhylands/deconz-dump-data/master/deconz-zcl-detail.log)
file was produced by adding the -d and -r options:
```
./dump.js -r -d ../../deconz-dump-data/deconz-zcl.json
```
