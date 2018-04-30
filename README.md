# IoT
Provide Various Codes for IoT applications

---------------------------------
---------------------------------
https://github.com/esp8266/arduino

http://www.c-sharpcorner.com/article/blinking-led-by-esp-12e-nodemcu-v3-module-using-arduinoide/

---------------------------------
---------------------------------

MQTT

Linux: 
http://pdacontrolen.com/installation-mosquitto-broker-mqtt-in/

Windows:
https://www.youtube.com/watch?v=xzHbMlFOu1E

s1: Admin Cmd :  Cd mosquitto -> mosquitto

s2: Admin Cmd :  Cd mosquitto -> mosquitto_sub -t topicname

s3: Admin Cmd :  Cd mosquitto -> mosquitto_pub -h 127.0.0.1 -p 1883 -t topicname -m "messsagehii"  
                              or  mosquitto_pub -h localhost -p 1883 -t test -m "mess"

---------------------------------
---------------------------------


	Copper Plugin (Install on old Firefox version)
-	Copper(Cu) plugin is not compatible with new Firefox.
-	Install any old version of Firefox version 45 to 50

	Install CoAP Library (https://github.com/automote/ESP-CoAP)

	Connect Temperature sensor with ESP8266	(Diagram is same as previous practical)

	Code for Copper url access: (For CoAP Server)
In Arduino IDE Go to file -> examples -> ESP-CoAP simple library ->  CoapServer 
We run above code to get the IP address of ESP

Now, Run the URI coap://IPaddress:default port number/resource to connect to ESP. 
  
	Code: (For GET and POST method)

Below two functions are used to control the actuators. 								                            The callback_temp will be used with GET method to get temperature                                                     	                          The callback_LED will be used with POST method to Turn on or Turn off led 
