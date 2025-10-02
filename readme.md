# Сборки Meshtastic для Heltec V3 с поддержкой кириллицы

Этот репозиторий автоматически собирает **прошивку Meshtastic** как только появляется новый стабильный или пре-релиз (альфа) с добавлением флага **-D OLED_RU**, в соответствии с документацией.

## Загрузка

Сборки публикуются в виде релизов. В комплект входят файлы .bin именованные в соответствии с версиями. Вариат factory - полная прошивка, без factory - обновление.

Всегда делайте резервную копию конфигурации перед прошивкой. 

## Прошивка
Пример (Linux/macOS):
```bash
esptool.py --chip esp32s3 --port /dev/cu.usbserial-0001 --baud 115200 write_flash -z 0x0 firmware.factory.bin
```

Любые действия с прошивкой вы выполняете на свой страх и риск.
Подробности в официальном гайде [тут](https://meshtastic.org/docs/getting-started/flashing-firmware/esp32/cli-script/)

---


# Meshtastic Heltec v3 Builds

This repository builds the **Meshtastic firmware** stable and pre-release for the  
**Heltec WiFi LoRa 32 v3 with OLED_RU flag** 

## Downloads
- Go to the [Releases page](../../releases) →  download the `heltec-v3-ru-###` binary file from the Assets of a release of your choice.
- Each artifact includes:
  - `firmware.bin`
  - `firmware.factory.bin`

## Flashing
Example (Linux/macOS):
```bash
esptool.py --chip esp32s3 --port /dev/cu.usbserial-0001 --baud 115200 write_flash -z 0x0 firmware.factory.bin
```


More info can be found in the [original docs](https://meshtastic.org/docs/getting-started/flashing-firmware/esp32/cli-script/)
