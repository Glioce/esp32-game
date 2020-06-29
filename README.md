# esp32-game

Se probaron 2 bootloaders: Odroid-Go y Esplay-Micro.  
Esplay-Micro  
Ventajas:  
+ Tiene más botones por lo que algunos juegos son más fáciles de usar (ej. Doom)  
+ Funciona en ESP32 con flash de 4MB  

Desventajas:  
+ Ocupa más pines para la tarjeta SD y para la salida de audio  
+ La salida de audio es digital, por lo que se necesita un DAC externo  
+ Los botones necesitan un módulo I2C externo  

Odroid-Go  
Ventajas:  
+ Utiliza pocos módulos externos (pantalla SPI, lector de SD, y amplificador de audio opcional)  
+ La pantalla y la SD comparten 3 pines SPI, se ahorran pines (la descripción de Esplay dice que esto puede causar problemas, pero hasta ahora no se han presentado)  
+ Salida de audio analógico directo del ESP32  
+ Tiene varios ports de juegos y launchers de emuladores  

Desventajas  
+ Necesita ESP32 con flash de al menos 8MB  

Se intentó usar la tarjeta de desarrollo Pycom Fipy 1.0, pero tiene pines ocultos que son necesarios.  
La tarjeta elegida para trabajar es ESP32-DevKitC-V4 (WROVER).  
Pinout:  
https://components101.com/microcontrollers/esp32-devkitc  

### Contribuciones a Odroid-Go  
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

Esquemático  
https://github.com/hardkernel/ODROID-GO/blob/master/Documents/ODROID-GO_REV0.1_20180518.pdf  
Otra consola basada en Odroid  
https://www.tindie.com/products/handheld-gaming/retro-esp32/  
Recompilar go-play  
https://forum.odroid.com/viewtopic.php?t=32081  
Datasheet PAM8304 monofónico
https://www.diodes.com/assets/Datasheets/PAM8304.pdf
Usaremos amplificador estéreo PAM8403

### Contribucioes a Esplay-Micro
https://github.com/pebri86/esplay-micro-firmware-collections
Datasheet DAC audio  
https://www.nxp.com/docs/en/data-sheet/UDA1334ATS.pdf  

## mejores instrucciones
Se instaló esp-idf en windows, pero el resultado fue peor.  
Se intentará en linux nuevamente. Estas instrucciones parecen resolver los problemas.  
https://forum.odroid.com/viewtopic.php?f=158&t=35558  
https://forum.odroid.com/viewtopic.php?f=158&t=35558  
https://forum.odroid.com/viewtopic.php?f=158&t=38651  
https://forum.odroid.com/viewtopic.php?f=158&t=33624  
https://docs.espressif.com/projects/esp-idf/en/v3.2.2/get-started/index.html#get-esp-idf  

## otra info
https://forum.pycom.io/topic/3134/using-pycom-boards-with-arduino-ide
https://docs.pycom.io/gitbook/assets/fipy-pinout.pdf

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

## LCD
Versión ISP  
http://www.lcdwiki.com/2.4inch_SPI_Module_ILI9341_SKU:MSP2402  
https://naylampmechatronics.com/blog/26_Tutorial-pantalla-TFT-t%C3%A1ctil-con-Arduino.html  


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



Otras consolas que usan ESP32

Game Wing
https://www.youtube.com/watch?v=Aw9cLeh3I_Y

DIY 10 players
https://www.youtube.com/watch?v=VvkpKVtYKmk

