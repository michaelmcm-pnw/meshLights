# meshLights

meshLights are social, wifi-connected lights with flexible LED effects. They were designed for loosely connected, small groups of people or vehicles to visually identify each other. Supports up to 6 nodes, with automatic mesh organization and synchronization of LED animation. Leverages FastLED and PainlessMesh projects, and adds leader election, display/effect logic, additional messaging functionality and error checking.

## Hardware & Materials

This software has been tested on ESP32 dev boards, specificially [this one](https://www.amazon.com/HiLetgo-ESP-WROOM-32-Development-Microcontroller-Integrated/dp/B0718T232Z?ref_=ast_sto_dp).  There are only a few hardware requirements, but because my implementation was designed to be mobile and robust, I've included optional build materials below too.

### Required components
* ESP32
* Addressable LED (eg. WS2811, WS2812) strip

Optional hardware components:
* [ESP32 DevKitC Wi-Fi and BLE LED Controller](https://www.evilgeniuslabs.org/esp32-devkitc-wi-fi-and-ble-led-controller) - daughterboard which mounts cleanly with the ESP32.  Makes it much easier to attach LED strand(s), and to use a barrel power connector.

### Software

A step by step series of examples that tell you how to get a development env running

Say what the step will be

## Built With

* [FastLED](https://github.com/FastLED/FastLED) - a library for easily & efficiently controlling a wide variety of LED chipsets.
* [painlessMesh](https://github.com/gmag11/painlessMesh) - a library that takes care of the particulars of creating a simple mesh network using esp8266 and esp32 hardware.
* [ArduinoJSON](https://github.com/bblanchon/ArduinoJson) - a C++ JSON library for Arduino and IoT (Internet Of Things).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

## Acknowledgments

* thanks to FastLED for the pre-built animations!
* Lots of inspiration and a bit of code from LED_Synch_Mesh_Send by Carl F Sutter (2017)
