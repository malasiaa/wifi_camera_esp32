# ESP32 Camera Web Server

This project sets up an ESP32 board with a camera module to stream live video over Wi-Fi. It uses the AI Thinker Model of the ESP32 camera and provides a web interface to view the stream.
The idea is to prove a concept of a security camera built with off the (my) shelf components :laughing:.

<p align="center">
  <img src="https://github.com/malasiaa/wifi_camera_esp32/assets/144847430/fca3089c-fa5a-4092-a673-106e22523507" width="300" height="300">
</p>

#### Requirements:

- PlatformIO (or Arduino IDE).
- ESP32 board with a camera module (AI Thinker Model) ([ESP32-CAM and ESP32-CAM-MB](https://pt.aliexpress.com/item/1005006938892262.html?src=google&src=google&albch=shopping&acnt=272-267-0231&slnk=&plac=&mtctp=&albbt=Google_7_shopping&gclsrc=aw.ds&albagn=888888&isSmbAutoCall=false&needSmbHouyi=false&src=google&albch=shopping&acnt=272-267-0231&slnk=&plac=&mtctp=&albbt=Google_7_shopping&gclsrc=aw.ds&albagn=888888&ds_e_adid=&ds_e_matchtype=&ds_e_device=c&ds_e_network=x&ds_e_product_group_id=&ds_e_product_id=pt1005006938892262&ds_e_product_merchant_id=5346350603&ds_e_product_country=PT&ds_e_product_language=pt&ds_e_product_channel=online&ds_e_product_store_id=&ds_url_v=2&albcp=20695431540&albag=&isSmbAutoCall=false&needSmbHouyi=false&gad_source=1&gclid=Cj0KCQjw4MSzBhC8ARIsAPFOuyUrv-3EmW35uy8ZSv-_7S-G1Faw_W5M5DSnsyVQwbEPoaeKBJvvBDEaAjWfEALw_wcB&aff_fcid=cf0879a328a44c42afd7b636f587dfdb-1718749467693-00217-UneMJZVf&aff_fsk=UneMJZVf&aff_platform=aaf&sk=UneMJZVf&aff_trace_key=cf0879a328a44c42afd7b636f587dfdb-1718749467693-00217-UneMJZVf&terminal_id=bec40578c234405895a1646236025a60&afSmartRedirect=y)).

<p align="center">
  <img src="https://github.com/malasiaa/wifi_camera_esp32/assets/144847430/a55c21e6-13be-4ac6-955c-7755ecd67221" width="200" height="200">
</p>
  
## Setup Instructions

- Open the Arduino IDE, or PlatformIO.
- Select the [main.cpp](https://github.com/malasiaa/wifi_camera_esp32/blob/main/main.cpp) file.
- Connect the ESP board to your computer.
- Select the appropriate board and port under Tools > Board and Tools > Port, or if using PlatformIO, upload the [config.ini](https://github.com/malasiaa/wifi_camera_esp32/blob/main/platformio.ini) file.
- Specify the SSID and password, in the main.cpp sketch.
 - Upload the code to the board.



