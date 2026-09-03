# thingboot-device · ThingBoot Device

[中文](README.md) | **English**

ThingBoot Device is the DEVICE-side development kit collection of the
[ThingBoot enterprise-grade IoT ecosystem and technical framework](https://github.com/ThingBoot/thingboot-iot).
It covers ESP (Espressif) chips — Arduino / ESP-IDF firmware SDKs — as well as
SDKs for Flutter / Go / HarmonyOS / Linux / Windows / Android platforms, with built-in WiFi, Ethernet,
4G Cat.1 and WiFi Mesh networking, out-of-the-box cloud connection and OTA support.

## Position in the Overall Architecture

```
thingboot-iot ThingBoot IoT Ecosystem
│
├── USER SIDE
│   ├── thingboot-web        ThingBoot Web
│   └── thingboot-client     ThingBoot Client
│
├── CLOUD SIDE
│   └── thingboot-cloud      ThingBoot Cloud Platform
│
└── DEVICE SIDE
    └── thingboot-device ★ this repository
        ├── thingboot-device-esp-arduino-sdk      ThingBoot Device ESP-Arduino SDK
        ├── thingboot-device-esp-idf-sdk          ThingBoot Device ESP-IDF SDK
        ├── thingboot-device-flutter-sdk          ThingBoot Device Flutter SDK
        ├── thingboot-device-go-sdk               ThingBoot Device Go SDK
        ├── thingboot-device-harmony-sdk          ThingBoot Device Harmony SDK (WIP)
        ├── thingboot-device-linux-sdk            ThingBoot Device Linux SDK (WIP)
        ├── thingboot-device-windows-sdk          ThingBoot Device Windows SDK (WIP)
        └── thingboot-device-android-sdk          ThingBoot Device Android SDK (WIP)
```

ThingBoot Device talks to the CLOUD-side [ThingBoot Cloud Platform](https://github.com/ThingBoot/thingboot-cloud) over MQTT / HTTPS;
in pure LAN mode it can also expose HTTP / TCP interfaces and run standalone.

## Sub-projects

| Repository | Description |
| --- | --- |
| [thingboot-device-esp-arduino-sdk](https://github.com/ThingBoot/thingboot-device-esp-arduino-sdk) | ThingBoot Device ESP-Arduino SDK, supporting ESP8266 / ESP32 / ESP32-S3 / ESP32-C6, with built-in WiFi, Ethernet, 4G Cat.1 and WiFi Mesh networking, out-of-the-box cloud connection and OTA |
| [thingboot-device-esp-idf-sdk](https://github.com/ThingBoot/thingboot-device-esp-idf-sdk) | ThingBoot Device ESP-IDF SDK, supporting ESP32 / ESP32-S3 / ESP32-C6 / ESP32-C3, with built-in WiFi, Ethernet, 4G Cat.1 and WiFi Mesh networking, out-of-the-box cloud connection and OTA, and an API consistent with the Arduino version |
| [thingboot-device-flutter-sdk](https://github.com/ThingBoot/thingboot-device-flutter-sdk) | ThingBoot Device Flutter SDK: turn Flutter apps (Android / iOS / desktop) into ThingBoot devices, with the same protocol & API as the Arduino SDK |
| [thingboot-device-go-sdk](https://github.com/ThingBoot/thingboot-device-go-sdk) | ThingBoot Device Go SDK: host/server-side device integration (soft gateways, edge services, cloud-side device simulators), wire-compatible with the C++ SDKs |
| [thingboot-device-harmony-sdk](https://github.com/ThingBoot/thingboot-device-harmony-sdk) | ThingBoot Device Harmony SDK (in development): connect HarmonyOS devices to ThingBoot Cloud |
| [thingboot-device-linux-sdk](https://github.com/ThingBoot/thingboot-device-linux-sdk) | ThingBoot Device Linux SDK (in development): connect Linux devices to ThingBoot Cloud |
| [thingboot-device-windows-sdk](https://github.com/ThingBoot/thingboot-device-windows-sdk) | ThingBoot Device Windows SDK (in development): connect Windows devices to ThingBoot Cloud |
| [thingboot-device-android-sdk](https://github.com/ThingBoot/thingboot-device-android-sdk) | ThingBoot Device Android SDK (in development): connect Android devices to ThingBoot Cloud |

## Related Repositories

- [thingboot-iot](https://github.com/ThingBoot/thingboot-iot): ThingBoot IoT ecosystem overview
- [thingboot-cloud](https://github.com/ThingBoot/thingboot-cloud): ThingBoot Cloud Platform
