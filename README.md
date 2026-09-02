# thingboot-device · 芯步设备端

**中文** | [English](README_EN.md)

芯步设备端是 [芯步（ThingBoot）企业级物联网生态与技术框架](https://github.com/ThingBoot/thingboot-iot) 设备侧的设备开发套件，
覆盖 ESP（乐鑫）系列芯片（Arduino / ESP-IDF 固件 SDK 及配套驱动）与 Flutter / HarmonyOS / Linux / Windows / Android 平台 SDK，
内置 WiFi、以太网、4G Cat.1 与 WiFi Mesh 组网能力，开箱即用直连芯步云平台并支持 OTA 升级。

## 在整体架构中的位置

```
thingboot-iot 芯步物联网生态
│
├── 用户侧
│   ├── thingboot-web        芯步 Web 端
│   └── thingboot-client     芯步客户端
│
├── 平台侧
│   └── thingboot-cloud      芯步云平台
│
└── 设备侧
    └── thingboot-device ★ 本仓库
        ├── thingboot-device-esp-arduino-sdk      芯步设备 ESP-Arduino SDK
        ├── thingboot-device-esp-arduino-drivers  芯步设备 ESP-Arduino 驱动
        ├── thingboot-device-esp-idf-sdk          芯步设备 ESP-IDF SDK
        ├── thingboot-device-esp-idf-driver       芯步设备 ESP-IDF 驱动
        ├── thingboot-device-flutter-sdk          芯步设备 Flutter SDK
        ├── thingboot-device-harmony-sdk          芯步设备 Harmony SDK（开发中）
        ├── thingboot-device-linux-sdk            芯步设备 Linux SDK（开发中）
        ├── thingboot-device-windows-sdk          芯步设备 Windows SDK（开发中）
        └── thingboot-device-android-sdk          芯步设备 Android SDK（开发中）
```

芯步设备端通过 MQTT / HTTPS 与平台侧的 [芯步云平台](https://github.com/ThingBoot/thingboot-cloud) 交互；
在纯局域网模式下亦可开放 HTTP / TCP 接口独立运行。

## 子项目

| 仓库 | 说明 |
| --- | --- |
| [thingboot-device-esp-arduino-sdk](https://github.com/ThingBoot/thingboot-device-esp-arduino-sdk) | 芯步设备 ESP-Arduino SDK，支持 ESP8266 / ESP32 / ESP32-S3 / ESP32-C6，内置 WiFi、以太网、4G Cat.1 与 WiFi Mesh 组网，开箱即用的平台直连与 OTA |
| [thingboot-device-esp-arduino-drivers](https://github.com/ThingBoot/thingboot-device-esp-arduino-drivers) | 芯步设备 ESP-Arduino 驱动 |
| [thingboot-device-esp-idf-sdk](https://github.com/ThingBoot/thingboot-device-esp-idf-sdk) | 芯步设备 ESP-IDF SDK，支持 ESP32 / ESP32-S3 / ESP32-C6 / ESP32-C3，内置 WiFi、以太网、4G Cat.1 与 WiFi Mesh 组网，开箱即用的平台直连与 OTA，接口与 Arduino 版保持一致 |
| [thingboot-device-esp-idf-driver](https://github.com/ThingBoot/thingboot-device-esp-idf-drivers) | 芯步设备 ESP-IDF 驱动 |
| [thingboot-device-flutter-sdk](https://github.com/ThingBoot/thingboot-device-flutter-sdk) | 芯步设备 Flutter SDK：让 Flutter 应用（Android / iOS / 桌面）作为设备接入芯步云平台，协议与接口和 Arduino 版一致 |
| [thingboot-device-harmony-sdk](https://github.com/ThingBoot/thingboot-device-harmony-sdk) | 芯步设备 Harmony SDK（开发中）：让鸿蒙 HarmonyOS 设备接入芯步云平台 |
| [thingboot-device-linux-sdk](https://github.com/ThingBoot/thingboot-device-linux-sdk) | 芯步设备 Linux SDK（开发中）：让 Linux 设备接入芯步云平台 |
| [thingboot-device-windows-sdk](https://github.com/ThingBoot/thingboot-device-windows-sdk) | 芯步设备 Windows SDK（开发中）：让 Windows 设备接入芯步云平台 |
| [thingboot-device-android-sdk](https://github.com/ThingBoot/thingboot-device-android-sdk) | 芯步设备 Android SDK（开发中）：让 Android 设备接入芯步云平台 |

## 相关仓库

- [thingboot-iot](https://github.com/ThingBoot/thingboot-iot)：芯步物联网生态总览
- [thingboot-cloud](https://github.com/ThingBoot/thingboot-cloud)：芯步云平台
