# node-red-contrib-meo-esp

This module provices a set of nodes in Node-RED to quickly receive data from ESP8266 board with MEO ESP firmware flashed.

There are 2 nodes available at the moment:
- An input node is to receive data from ESP Board, bellow is a sample of output format:
```json
{
  "deviceId": "DEVICE_ID",
  "payload": {
    "D5": 0,
    "D6": 1,
    "D7": 1,
    "D8": 0,
    "A0": 129,
    "V1": undefined,
    "V2": undefined,
    "V3": undefined,
    "V4": undefined,
    "V5": undefined
  }
}
```

- An ouput node is to send configuration to target ESP Board, users can set the value from pin D0 to D5 (HIGH, LOW or PWM)

## Pre-requisites

Node-RED-MEO-ESP requires Node-RED version 0.14 or more recent.

## Install

To install the stable version run the following command in your Node-RED user directory (typically `~/.node-red`):

    npm i node-red-contrib-meo-esp

Open your Node-RED instance and you should have one new node in input category and one new node in output category.
