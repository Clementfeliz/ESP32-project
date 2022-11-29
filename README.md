# ESP32-Camera WebServer

## Equipment used:

### -ESP32 CAM : https://www.amazon.com/gp/product/B097BLT24K/ref=ppx_yo_dt_b_asin_title_o02_s00?ie=UTF8&amp=undefined&th=1
### -USB cable: https://www.amazon.com/AmazonBasics-Male-Micro-Cable-Black/dp/B07232M876/ref=sr_1_3?crid=3V5R563NM84Z2&keywords=usb+2.0+a-male+to+micro+b+cable&qid=1669682125&s=electronics&sprefix=usb+2%2Celectronics%2C89&sr=1-3

## Software: Legacy IDE (1.8.X)
### https://www.arduino.cc/en/software

## Source:
### https://randomnerdtutorials.com/installing-the-esp32-board-in-arduino-ide-windows-instructions/
### https://youtu.be/mBaS3YnqDaU
### https://youtu.be/RCtVxZnjPmY

## Configuring the ESP32 board on the Arduino:
### 1-After installing Arduino IDE, go to FILE > click on “PREFERENCE”.
### 2- On the Preferences screen, fill the following link into the ‘Additional board manager URLS’:
https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json
### 3-Press Ok
### 4- Go to TOOLS > BOARD: > and then click on “BOARDS MANAGER…”.
### 5- Type “esp32” on the filter your search and install the latest version available. At this moment is version 2.0.5. 
### 6-Go to TOOLS > BOARD: > ESP32 ARDUINO > and click on “AI THINKER ESP32-CAM”. 
### 7- Go to FILE > EXAMPLES > ESP32 > CAMERA> and click CAMERAWEBSERVER  
-Note: Please select the port: COM that the esp32 was detected on. If you are not sure disconnect the esp32 and check the port: COM available. And the reconnect the esp32 and the new port that appears is the one you should select on the configuration. In my case the Esp32 was detected on COM 8.  

-Note: Please verify line 24 #define CAMARA_MODEL_AI_THINKER
### 8- Go to line #36 (SSID) and #37 (PASSWORD) to type the credentials of the network that you want the Esp32 Webcam connected to. Note: Insert your credentials inside the Ellipsis “CREDENTIALS”, remember to delete the stars, because only your credentials should be inside the Ellipsis. 
### 9- Press the upload button to upload the configuration and after the upload is done press the Serial Monitor  
### 10- A new tap with the port number will appear. Please press the reset button on the esp32 card and the camera IP address will be shown. Then use your browser to go to the camera IP address. Note: The devices must be on the same network. If not on the same network ‘Port forwarding must be active on the camera server network’ for remotely connection. 

### 11-Press the Start Stream on the Advance settings to start the life stream. 



