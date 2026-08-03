# thingboot-device · ThingBoot Device

[中文](README.md) | **English**

ThingBoot Device is the device-side development kit collection of the
[ThingBoot IoT ecosystem](https://github.com/ThingBoot/thingboot-iot).
The kits run on ESP (Espressif) chips and provide firmware SDKs in both Arduino-framework
and ESP-IDF versions together with matching drivers, with built-in WiFi, Ethernet,
4G Cat.1 and WiFi Mesh networking, out-of-the-box cloud connection and OTA support.

## Position in the Overall Architecture

```
thingboot-iot ThingBoot IoT Ecosystem
│
├── Upper Layer
│   ├── thingboot-web        ThingBoot Web
│   ├── thingboot-client     ThingBoot Client
│   └── thingboot-device ★ this repository
│       ├── thingboot-device-esp-arduino-sdk      ESP Arduino firmware SDK
│       ├── thingboot-device-esp-arduino-drivers  ESP Arduino drivers
│       ├── thingboot-device-esp-idf-sdk          ESP-IDF firmware SDK
│       └── thingboot-device-esp-idf-sdk-driver   ESP-IDF drivers
│
└── Cloud Layer
    └── thingboot-cloud      ThingBoot Cloud Platform
```

ThingBoot Device talks to the underlying [ThingBoot Cloud Platform](https://github.com/ThingBoot/thingboot-cloud) over MQTT / HTTPS;
in pure LAN mode it can also expose HTTP / TCP interfaces and run standalone.

## Sub-projects

| Repository | Description |
| --- | --- |
| [thingboot-device-esp-arduino-sdk](https://github.com/ThingBoot/thingboot-device-esp-arduino-sdk) | ESP Arduino firmware SDK supporting ESP8266 / ESP32 / ESP32-S3 / ESP32-C6, with built-in WiFi, Ethernet, 4G Cat.1 and WiFi Mesh networking, out-of-the-box cloud connection and OTA |
| [thingboot-device-esp-arduino-drivers](https://github.com/ThingBoot/thingboot-device-esp-arduino-drivers) | ESP Arduino drivers |
| [thingboot-device-esp-idf-sdk](https://github.com/ThingBoot/thingboot-device-esp-idf-sdk) | ESP-IDF firmware SDK, a port of the Arduino SDK above, supporting ESP32 / ESP32-S3 / ESP32-C6 / ESP32-C3, with an API highly consistent with the Arduino version |
| [thingboot-device-esp-idf-sdk-driver](https://github.com/ThingBoot/thingboot-device-esp-idf-sdk-driver) | ESP-IDF drivers |

## Related Repositories

- [thingboot-iot](https://github.com/ThingBoot/thingboot-iot): ThingBoot IoT ecosystem overview
- [thingboot-cloud](https://github.com/ThingBoot/thingboot-cloud): ThingBoot Cloud Platform
