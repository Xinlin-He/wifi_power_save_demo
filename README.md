# Wi-Fi Power Save Configuration

- [中文版](./README_CN.md)

### Project Overview

This project is based on the Espressif official Wi-Fi Power Save example and provides a custom sdkconfig file. By adjusting Wi-Fi low-power related configuration options, the project targets the lowest possible power consumption.

This configuration file only modifies configuration options and does not change any source code logic.
When using this configuration, Wi-Fi power consumption on ESP32 series chips can be significantly reduced; however, it may impact communication timeliness and reliability, such as increased latency or packet loss.

### Usage

Run the following commands to switch to the target sdkconfig file:

- export SDKCONFIG_DEFAULTS="sdkconfig.s3"
- idf.py build