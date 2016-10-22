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

# Request

This plugin will call the specified URL for both On and Off state. It expects the server, that receives the request, to toggle the state for each subsequent call.

# Response

The plugin expects to receive a JSON body for all responses <= 400 HTTP Status code. It discards the body of the responses for HTTP status codes > 400 and will treat it as an error.
