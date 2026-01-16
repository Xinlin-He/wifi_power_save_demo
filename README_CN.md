# Wi-Fi Power Save Configuration

- [English](./README.md)

### 项目简介

本项目基于 Espressif 官方 Wi-Fi Power Save 示例修改生成了一个自定义 sdkconfig 文件，通过调整 Wi-Fi 低功耗相关配置，实现最低功耗模式。
此配置文件仅修改了配置项，未改动任何源代码逻辑。
使用该配置文件时，ESP32 系列芯片可显著降低 Wi-Fi 相关功耗，但可能会对数据通信的实时性和可靠性产生影响，例如增加延迟或出现丢包。

### 使用方法

输入以下指令修改至目标 sdkconfig 文件：

- export SDKCONFIG_DEFAULTS="sdkconfig.s3"
- idf.py build