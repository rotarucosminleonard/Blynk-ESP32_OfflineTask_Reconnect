# Blynk-ESP32_OfflineTask_Reconnect

Connection management on Blynk plarform for ESP32. Diagnose the connection issue, run a task online or offline

This sketch is based on an example posted by Gunner with some modifications added in place to make it able to reconnect after Wifi or Server connection failures.
It is able to check if it is a Wifi or a server connection issue and recover it when it is possible.
The MCU runs the task every second whether it is online or not - It turns the builtin led on and off (allways) and attempts to post the millis/1000 to blynk server if there is a connection to the server..
