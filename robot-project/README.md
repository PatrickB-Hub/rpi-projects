# Webcontrolled RPI ROBOT

Raspberry Pi robot with 4 motors attached to the wheels and additional servo motors to tilt and pan the camera that is mounted on top (plus an optional light mounted to the camera).
The RPI acts as a server accepting inputs from the client and it streams the camera image which is displayed on the clientside (website). 
The server runs the CGI script that is being requested over a GET request by the client. 

It uses the wiringPi library to access the GPIO via shell commands. 
The lighttpd library to run the rpi server https://www.lighttpd.net/
As well as the mjpg-streamer to transmit the camera image over the network.

Download the mjpg-streamer https://sourceforge.net/projects/mjpg-streamer/.
Follow the installation instructions.