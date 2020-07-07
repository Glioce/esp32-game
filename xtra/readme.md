
Esta carpeta contine dos programas para probar LCD TFT en Arduino.  

## Otras consolas que usan ESP32
Game Wing
https://www.youtube.com/watch?v=Aw9cLeh3I_Y

DIY 10 players
https://www.youtube.com/watch?v=VvkpKVtYKmk

esp-8-bit
https://github.com/rossumur/esp_8_bit  

Se intentó usar la tarjeta de desarrollo Pycom Fipy 1.0, pero tiene pines ocultos que son necesarios.  
La tarjeta utilizada para las primeras pruebas es ESP32-DevKitC-V4 (WROVER 4MB).  
Pinout:  
https://components101.com/microcontrollers/esp32-devkitc  
Las versiones antiguas de Odroid (con terminación psram) funcionan en ESP32 WROVER con memoria de 4 MB.
https://wiki.odroid.com/odroid_go/firmware_update_oldfw

Se usará un ESP32 con 16MB castelado para el dispositivo final  
https://www.mouser.mx/ProductDetail/Espressif-Systems/ESP32-WROVER-B-16MB?qs=sGAEpiMZZMu3sxpa5v1qrgLFJPTQ7Q2r6%2Fk%2Fforxl60=  
https://www.mouser.mx/ProductDetail/Espressif-Systems/ESP32-WROVER-IB-16MB?qs=sGAEpiMZZMu3sxpa5v1qrgLFJPTQ7Q2raQ%252Bbp2DOsnE%3D  
8MB  
https://www.mouser.mx/ProductDetail/Espressif-Systems/ESP32-WROVER-B-8MB?qs=sGAEpiMZZMu3sxpa5v1qrgLFJPTQ7Q2rs709VLUkb90%3D  
https://www.mouser.mx/ProductDetail/Espressif-Systems/ESP32-WROVER-IB-8MB?qs=sGAEpiMZZMu3sxpa5v1qrgLFJPTQ7Q2rhiPGTUzM78o%3D  
La terminación "-B" indica Meandered Inverted-F Antenna  
https://en.wikipedia.org/wiki/Inverted-F_antenna  
La terminación "-IB" indeca U.FL Antenna  
https://en.wikipedia.org/wiki/Hirose_U.FL  

## Contribuciones a Odroid-Go  
https://github.com/32teeth  
https://github.com/retro-esp32/RetroESP32  
https://github.com/retro-esp32/Retro-Odroid-Go-Firmware  
Descripción general y cómo empezar  
https://wiki.odroid.com/odroid_go/odroid_go  
Cómo actualizar firmware  
https://wiki.odroid.com/odroid_go/firmware_update  
https://github.com/OtherCrashOverride/go-play
Make SD card  
https://wiki.odroid.com/odroid_go/make_sd_card  
Colecciones de aplicaciones  
https://forum.odroid.com/viewtopic.php?f=159&t=31716  
https://github.com/chrisdiana/awesome-odroid-go  
https://www.reddit.com/r/OdroidGo/comments/gk9l2w/collection_of_os_images_for_odroid_go_and_odroid/  

## Contribucioes a Esplay-Micro
https://github.com/pebri86/esplay-micro-firmware-collections
Datasheet DAC audio  
https://www.nxp.com/docs/en/data-sheet/UDA1334ATS.pdf  
