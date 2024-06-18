# ESP32 Camera Web Server

This project sets up an ESP32 board with a camera module to stream live video over Wi-Fi. It uses the AI Thinker Model of the ESP32 camera and provides a web interface to view the stream.

<p align="center">
  <img src="https://github.com/malasiaa/arduino_temp-moist_sensing/assets/144847430/dac9f37d-082f-4541-9053-d377375ca0bf" width="400" height="200">
</p>

## Overview

The sketch was done on VS Code IDE with PlatformIO extension, with the config file [platformio.ini](https://github.com/malasiaa/wifi_camera_esp32/blob/main/platformio.ini).

Library Inclusions and GPIO Definitions:

Includes libraries for camera operations, Wi-Fi management, HTTP server, and other essential functions.
Defines the GPIO pins specific to the AI Thinker model for the camera connections.

Network Credentials:

Specifies the SSID and password for connecting to a Wi-Fi network.

Antenna Configuration:

Sets up GPIO12 to use an external antenna for better Wi-Fi reception.

Camera Configuration:

Configures the camera settings, including frame size, JPEG quality, and GPIO pins for various camera functions.
Handles the initialization of the camera and checks for errors.
HTTP Server Setup:

Configures an HTTP server to handle video streaming requests.
Sets the content type for multipart JPEG streaming and defines the HTTP response structure.
Stream Handler Function:

Captures frames from the camera.
Converts frames to JPEG if necessary.
Sends the JPEG frames as chunks over HTTP to the connected client.
Manages the buffer and handles any errors during the frame capture and sending process.

Server Initialization:

Initializes the HTTP server and registers the URI handler for the root path to handle video streaming requests.

Wi-Fi Connection:

Connects the ESP32 to the specified Wi-Fi network.
Waits until a connection is established and then prints the IP address to the Serial Monitor.

Main Functions:

setup(): Initializes the camera, configures the GPIO for the antenna, sets up the Wi-Fi connection, and starts the HTTP server.
loop(): Contains a minimal loop to keep the program running.

#### Components Used:

- ESP32 board with a camera module (AI Thinker Model) ([ESP32-CAM and ESP32-CAM-MB](https://pt.aliexpress.com/item/1005006938892262.html?src=google&src=google&albch=shopping&acnt=272-267-0231&slnk=&plac=&mtctp=&albbt=Google_7_shopping&gclsrc=aw.ds&albagn=888888&isSmbAutoCall=false&needSmbHouyi=false&src=google&albch=shopping&acnt=272-267-0231&slnk=&plac=&mtctp=&albbt=Google_7_shopping&gclsrc=aw.ds&albagn=888888&ds_e_adid=&ds_e_matchtype=&ds_e_device=c&ds_e_network=x&ds_e_product_group_id=&ds_e_product_id=pt1005006938892262&ds_e_product_merchant_id=5346350603&ds_e_product_country=PT&ds_e_product_language=pt&ds_e_product_channel=online&ds_e_product_store_id=&ds_url_v=2&albcp=20695431540&albag=&isSmbAutoCall=false&needSmbHouyi=false&gad_source=1&gclid=Cj0KCQjw4MSzBhC8ARIsAPFOuyUrv-3EmW35uy8ZSv-_7S-G1Faw_W5M5DSnsyVQwbEPoaeKBJvvBDEaAjWfEALw_wcB&aff_fcid=cf0879a328a44c42afd7b636f587dfdb-1718749467693-00217-UneMJZVf&aff_fsk=UneMJZVf&aff_platform=aaf&sk=UneMJZVf&aff_trace_key=cf0879a328a44c42afd7b636f587dfdb-1718749467693-00217-UneMJZVf&terminal_id=bec40578c234405895a1646236025a60&afSmartRedirect=y)).
- Arduino IDE or PlatformIO.
#### Circuit Design:

<p align="center">
  <img src="" width="400" height="400">
</p>

#### ESP32-CAM Setup:



## Setup Instructions
