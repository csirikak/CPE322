## Lab 5 — Paho-MQTT
### Install Mosquitto
https://mosquitto.org/files/binary/win64/mosquitto-2.0.15-install-windows-x64.exe \
Make sure to add mosquitto to PATH\
Ensure mosquitto is started as a service or in a terminal
### Install paho-mqtt
```
pip install paho-mqtt
```
### client
```
py client.py
Connected with result code 0
$SYS/broker/publish/bytes/received 517360038195
$SYS/broker/publish/bytes/sent 17335093225529
$SYS/broker/publish/messages/dropped 2012487563197
$SYS/broker/publish/messages/received 3982896015
$SYS/broker/publish/messages/sent 133781563959
$SYS/broker/publish/messages/dropped 2012488207130
$SYS/broker/publish/messages/received 3982920568
$SYS/broker/publish/messages/sent 133782332430
$SYS/broker/publish/bytes/received 517363614434
$SYS/broker/publish/bytes/sent 17335196059775
$SYS/broker/publish/messages/dropped 2012488768318
$SYS/broker/publish/messages/received 3982942707
$SYS/broker/publish/messages/sent 133783023780
$SYS/broker/publish/bytes/received 517368458255
$SYS/broker/publish/bytes/sent 17335301302015
```
## Run the following on separate terminals
### Terminal 1
```
py sub.py
Connected with result code 0
paho/test Hello
```
### Terminal 2
```
py pub.py
```
### Terminal 1
```
py sub-multiple.py
Connected with result code 0
paho/test/multiple multiple 1
paho/test/multiple multiple 2
```
### Terminal 2
```
py pub-multiple.py
```
### Terminal 1
```
py subcpu.py
Connected with result code 0
MyCPU 2023-04-03 11:37:29
MyCPU CPU Usage:   1.6 %
```
### Terminal 2
```
py pubcpu.py
2023-04-03 11:37:29
CPU Usage:   1.6 %
```
