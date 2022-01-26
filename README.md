# HID-MQTT bridge

Original work from martonperei, i've mostly just removed the bluetooth portion of this and made this as a starter project for 
removing all dependencies on the harmony hub. 

Ultimately, i'd like to provide a good way for all buttons on the harmony hub to be easily configurable. perhaps through a custom component.

## Requirements

* sudo apt install libpaho-mqtt-dev liblua5.3-dev libusb-1.0-0-dev libudev-dev

## Building

* git clone --recursive git@github.com:martonperei/mqtt-hid-bridge.git
* cd mqtt-hid-bridge && sudo make install

## Usage

* /usr/local/bin/usb-hid-mqtt -a tcp://mqtt.local.lan -t usb-hid -u user -p pass
