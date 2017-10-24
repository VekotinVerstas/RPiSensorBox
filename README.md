# Raspberry Pi sensor box, exposes sensor readings as a BLE service

The box can have any sensors connected but you must write scripts for reading them and publishing the results to a local MQTT queue. A Node.js [application](rpi-ble-services) exposes these readings as a Bluetooth Smart / BLE service.

Scripts for reading BME280 and SDS011 sensors (temperature/humidity/barometric pressure and PM2.5/PM10 particulate counts, respectively) are provided in the [mqtt-sensors](mqtt-sensors) folder.


### Installation
Set up the OS and install the Node.js-BLE app as shown in the [rpi-ble-services](rpi-ble-services) directory.

Connect the sensors and install the python scripts for reading them. Instructions in the [mqtt-sensors](mqtt-sensors) directory ([general README](mqtt-sensors/README.md) and [bme280.md](mqtt-sensors/bme280.md)).

Some more information about wiring the sensors and the use of the [companion Android application](https://github.com/City-of-Helsinki/bt2cloud) (direct link to installer [HERE](https://github.com/City-of-Helsinki/bt2cloud-app/releases/download/v1.0.0rc/bt2cloud-release_v1.0.0rc.apk)) can be found in https://github.com/VekotinVerstas/rpi-air-workshop.
