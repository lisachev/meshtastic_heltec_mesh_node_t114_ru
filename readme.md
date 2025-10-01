# Meshtastic Heltec v2 Builds

This repository builds the **Meshtastic firmware** stable and pre-release for the  
**Heltec WiFi LoRa 32 v3 with OLED_RU flag** 

## Downloads
- Go to the [Actions tab](../../actions) → click the latest run → download the `heltec-v3-pre-###` or `heltec-v3-###` artifact.
- Each artifact includes:
  - `firmware.bin`
  - `firmware.factory.bin`
- Or go to releases

## Flashing
Example (Linux/macOS):
```bash
esptool.py --chip esp32 --port /dev/ttyUSB0 write_flash -z 0x0 firmware.factory.bin
```


More info can be found in the [original docs](https://meshtastic.org/docs/getting-started/flashing-firmware/esp32/cli-script/)
