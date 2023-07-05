# MPU6050 Cemuhook gyro

Gyroscope for Cemuhook, based on ESP8266 microcontroller and MPU6050 accelerometer and gyroscope IC

<img src="https://github.com/KerJoe/MPU6050-Cemuhook-gyro/raw/master/demo.png" width="300">

Instructions for use :
From https://github.com/jrowberg/i2cdevlib - download and install I2Cdev and MPU6050 libraries.
Download and install this library - https://github.com/bakercp/CRC32
Also this for the LEDs - https://github.com/FastLED/FastLED

Run calibrate.ino first. Follow instructions on screen. Then copy the result it gives you and replace the corresponding code in gyro.ino. Enter your WiFi SSID and Password in the given section. You will need to check your WiFi router to find the IP address of the ESP. You can use the IP for motion input in any program.

Code uses a WS2812 LED on GPIO12 for showing status. Orange blinking while searching for WiFi, solid green once connected and running. Red blinking if MPU6050 is not connected.
