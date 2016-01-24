# homebridge-http-simple-switch

Supports https devices on HomeBridge Platform

# Installation

1. Install homebridge using: npm install -g homebridge
2. Install this plugin using: npm install -g homebridge-http-simple-switch
3. Update your configuration file. See sample-config.json in this repository for a sample. 

# Configuration



Configuration sample:

 ```
"accessories": [
        "accessories": [
        {
            "accessory": "SimpleHttpSwitch",
            "name": "Living Room Button",
            "url": "http://192.168.1.210/button",
            "default_state_off": true, 
            "sendimmediately": "",
            "http_method": "GET"
        }
    ]

```# homebridge-http-simple-switch
