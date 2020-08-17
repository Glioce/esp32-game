Esta carpeta contine dos programas para probar LCD TFT paralelo en Arduino.  

## Otras consolas que usan ESP32
Game Wing
https://www.youtube.com/watch?v=Aw9cLeh3I_Y

DIY 10 players
https://www.youtube.com/watch?v=VvkpKVtYKmk

esp-8-bit
https://github.com/rossumur/esp_8_bit  

MCUME  
https://github.com/Jean-MarcHarvengt/MCUME  

https://neonaut.neocities.org/blog/2020/gaming-with-the-esp32.html  
https://hackaday.io/project/163464-gaming-on-the-esp32-odroid-go  

En este instructable instalan memoria extra en el ESP32  
https://www.instructables.com/id/Homemade-Odroid-go-Compatible-Game-Console/  

Se intentó usar la tarjeta de desarrollo Pycom Fipy 1.0, pero tiene pines ocultos que son necesarios.  
La tarjeta utilizada para las primeras pruebas es ESP32-DevKitC-V4 (WROVER 4MB).  
Pinout:  
https://components101.com/microcontrollers/esp32-devkitc  

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


## Contribucioes a Esplay-Micro
https://github.com/pebri86/esplay-micro-firmware-collections
Datasheet DAC audio  
https://www.nxp.com/docs/en/data-sheet/UDA1334ATS.pdf  

## otra info
https://forum.pycom.io/topic/3134/using-pycom-boards-with-arduino-ide
https://docs.pycom.io/gitbook/assets/fipy-pinout.pdf
https://hackaday.io/project/163464-gaming-on-the-esp32-odroid-go  
https://www.instructables.com/id/Homemade-Odroid-go-Compatible-Game-Console/  
https://neonaut.neocities.org/blog/2020/gaming-with-the-esp32.html  

ESPlay  

Resumen / venta ESPlay  
https://www.makerfabs.com/esplay-micro.html  

Página de ESPlay en Hackaday  
https://hackaday.io/project/166707-esplay-micro  

Review ESPlay  
https://www.youtube.com/watch?v=NfbxcjU85Ac  

Repositorios ESPlay  
Colección de emuladores  
https://github.com/pebri86/esplay-retro-emulation  
Hardware (PCB)  
https://github.com/pebri86/esplay_micro_hardware  
Base firmware  
https://github.com/pebri86/esplay-base-firmware  
Firmware release  
https://github.com/pebri86/esplay-base-firmware/releases/tag/v1.0-esplay-micro  
Firmware collections  
https://github.com/pebri86/esplay-micro-firmware-collections  

Info fipy  
https://docs.pycom.io/datasheets/development/fipy/  
https://medium.com/home-wireless/the-pycom-lopy-long-range-transceiver-d8d80622adee  
Pinout fipy  
https://docs.pycom.io/datasheets/development/fipy/  

Info ESP32 Wrover  
https://www.14core.com/wiring-bootloading-and-flashing-the-espressif-esp32-wrover/  

Usar TFT LCD con Arduino  
https://electropeak.com/learn/absolute-beginners-guide-to-tft-lcd-displays-by-arduino/  
https://electropeak.com/learn/arduino-2-4-touch-screen-lcd-shield-tutorial/  
https://www.instructables.com/id/How-to-use-24-inch-TFT-LCD-SPFD5408-with-Arduino-U/  
https://electronicavm.wordpress.com/2015/03/05/tft-lcd-touch-2-4-shield-para-arduino-uno/  

Pantalla LCD TFT  
Esta se compró primero pero usa comunicación en paralelo (8 bits)  
http://www.lcdwiki.com/2.4inch_Arduino_Display  
Viene configurada desde adentro, en los pines del flexo (ribbon cable) solo se pueden acceder a otros pines paralelos  
http://www.lcdwiki.com/Main_Page  
Responder en Foro que no se puede cambiar el bus  
https://forum.arduino.cc/index.php?topic=357982.0  

Búsqueda de pantallas  
Para RPi ili9341  
https://www.geekfactory.mx/tienda/raspberry-pi/shield-pantalla-lcd-tactil-2-8-pulgadas-para-raspberry-pi-itead/  
http://madrigalelectronics.com/raspberry-pi-4b-3b-2.8-inch-touchscreen-tft-spi-display-with-touch-pen.html?currency=MXN  
https://hetpro-store.com/lcd-tft-2.8-touch-resistivo-para-raspberry-pi-stmpe610ili9341/  

Posible  
https://sandorobotics.com/producto/im140714002/  
https://www.electronicaestudio.com/tienda/robotica-estudio/pantalla-2-4-tactil-serial/  
http://madrigalelectronics.com/3.2-tft-lcd-shield--touch-panel-tf-reader-for-arduino.html?currency=MXN

Perfecta
https://articulo.mercadolibre.com.mx/MLM-553195850-lcd-serial-spi-22-240x320-pixeles-socket-sd-ili9341-qvga-_JM  

## Historia de Arcades de Nintendo  
https://tiredoldhack.com/2017/09/16/the-complete-history-of-nintendo-arcade-games/  

## Software compatible con ESPlay  
## mejores instrucciones
Se instaló esp-idf en windows, pero el resultado fue peor.  
Se intentará en linux nuevamente. Estas instrucciones parecen resolver los problemas.  
https://forum.odroid.com/viewtopic.php?f=158&t=35558  
https://forum.odroid.com/viewtopic.php?f=158&t=35558  
https://forum.odroid.com/viewtopic.php?f=158&t=38651  
https://forum.odroid.com/viewtopic.php?f=158&t=33624  
https://docs.espressif.com/projects/esp-idf/en/v3.2.2/get-started/index.html#get-esp-idf  

## cerca de compilar
El problema actual es no poder construir/compilar esplay-base-firmware  
(ver releases)  
https://github.com/pebri86/esplay-base-firmware

Platformio puede servir  
https://docs.platformio.org/en/latest/boards/espressif32/odroid_esp32.html  
Zephyr?  
https://docs.zephyrproject.org/latest/boards/xtensa/odroid_go/doc/index.html  

Foro de odroid. Solucionan error en windows  
https://forum.odroid.com/viewtopic.php?f=158&t=35558  

Artículos complicados instalar esp-idf  
https://medium.com/@jungpil.yu/esp-idf-based-development-environment-for-odroid-go-e27ff41b4adf  
https://lerks.blog/build-apps-for-odroid-go-using-esp-idf/  

Versión parchada esp-idf  
https://github.com/OtherCrashOverride/esp-idf  
v3.2-odroid  
https://github.com/OtherCrashOverride/esp-idf/tree/release/v3.2-odroid  

Doc oficial esp-idf  
Instalar toolchain  
https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/linux-setup.html  
Get started  
https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/index.html  
Get satarted 4.0.1  
https://docs.espressif.com/projects/esp-idf/en/stable/get-started/  

Página de esplay en hackaday  
https://hackaday.io/project/166707-esplay-micro  

Repo de retro-emulation tiene instrucciones de compilación  
https://github.com/pebri86/esplay-retro-emulation  