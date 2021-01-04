# meshLights

meshLights are social, wifi-connected lights with flexible LED effects. They were designed for loosely connected, small groups of people or vehicles to visually identify each other. Supports up to 6 nodes, with automatic mesh organization and synchronization of LED animation. Leverages FastLED and PainlessMesh projects, and adds leader election, display/effect logic, additional messaging functionality and error checking.

## Hardware & Materials

This software has been tested on the Hiletgo ESP-WROOM-32 ESP32 dev boards.  There are only a few hardware requirements, but because my implementation was designed to be mobile and robust, I've included optional build materials below too.

### Required components
* [**ESP32 2.4GHz Dual-Mode WiFi + Bluetooth Dual Cores Microcontroller**](https://www.amazon.com/HiLetgo-ESP-WROOM-32-Development-Microcontroller-Integrated/dp/B0718T232Z?ref_=ast_sto_dp) - tested with the Hiletgo ESP-WROOM-32 ESP32 dev board. [Hiletgo details](http://hiletgo.com/ProductDetail/1906566.html)
* [**Addressable LED strip**](https://www.amazon.com/gp/product/B01MQ08JH6/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1) (eg. WS2811, WS2812) - tested with WS8212B strands with 30, 60 & 120 LEDs.

Optional hardware components:
* [**ESP32 DevKitC Wi-Fi and BLE LED Controller**](https://www.evilgeniuslabs.org/esp32-devkitc-wi-fi-and-ble-led-controller) - daughterboard which mounts cleanly with the ESP32.  Makes it much easier to attach LED strand(s), and to use a barrel power connector.

### Software
* To build / upload the code to your ESP32, use [Microsoft's VS Code](https://code.visualstudio.com/) with the [PlatformIO extension](https://platformio.org/) or Arduino IDE.  Both have been tested, and work.

## Built With

* [FastLED](https://github.com/FastLED/FastLED) - a library for easily & efficiently controlling a wide variety of LED chipsets.
* [painlessMesh](https://github.com/gmag11/painlessMesh) - a library that takes care of the particulars of creating a simple mesh network using esp8266 and esp32 hardware.
* [ArduinoJSON](https://github.com/bblanchon/ArduinoJson) - a C++ JSON library for Arduino and IoT (Internet Of Things).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

## Acknowledgments

* thanks to FastLED for the pre-built animations!
* Lots of inspiration and a bit of code from LED_Synch_Mesh_Send by Carl F Sutter (2017)
