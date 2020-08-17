# Software de Mini Arcade
Esta es una lista de software compatible con Odroid-go.
La información de software compatible con ESPlay está en la carpeta "xtra".  

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

## Bootloader  
Las versiones antiguas de Odroid (con terminación psram) 
funcionan en ESP32 WROVER con memoria de 4 MB.  
https://wiki.odroid.com/odroid_go/firmware_update_oldfw  

La versión estándar funciona bien en ESP32 WROVER 16 MB.  
El build más reciente es 20181001  
https://github.com/OtherCrashOverride/odroid-go-firmware/releases

Multi-firmware. Instala múltiples aplicaciones en flash.  
Solo se ha probado una vez (Build 20190901), ¿en verdad tiene ventajas?  
https://github.com/ducalex/odroid-go-multi-firmware  

## Aplicaiones    
Lanzadores de emuladores y otras aplicaciones.  

### Probados  
Go-play lanzador oficial  
Casi no se notan diferencias entre builds. Han mejorado compatibilidad de tarjetas SD.  
El build más reciente es 20181004. Tiene 6 emuladores.  
https://forum.odroid.com/viewtopic.php?f=159&t=31348  

Super Go-play  
Se parece a Go-play estandar.
Usa combinaciones de botones para volumen y paleta de colores de GB.  
https://github.com/mattkj/super-go-play  

Retro-go  
Agrega muchas características. Hay muchas opciones de configuración.  
Versión que funcionó 2020-08-01. Tiene 8 emuladores.  
https://github.com/ducalex/retro-go  

Nes multiplayer  
La consola no muestra errores, pero la pantalla se queda en blanco.
Probar con 2 instancias al mismo tiempo.  
https://github.com/OtherCrashOverride/nes-mp-go/releases  

Doom  
¿Guarda partidas?  


Teclado BT  
Funciona con un celular. El joystick permite navegar,
A parece tecla Enter, B parece tecla Back. ¿Qué hacen los otros botones?  
https://github.com/ripper121/odroidgoupdater  

### No probados  
RetroESP32
No ha funcionado. Cuando termina de instalarse, el ESP32 se reinicia.  
Se ha intentado con varias versiones (hasta v2.5).  
¿Por qué no funciona?  
- ¿ESP32 es diferente al que usa Odroid?
- ¿Se dañó la memoria?
- ¿Falla la fuente de alimentación?
- ¿Se necesita un bootloader especial?
- ¿Hay Efuses que impiden la ejecución?
- ¿Faltan archivos o carpetas en la SD?
- ¿Se necesita pull-up o pull-down en algún pin?  
https://github.com/retro-esp32/RetroESP32  
https://wiki.odroid.com/odroid_go/emulator/retro_esp32  
https://forum.odroid.com/viewtopic.php?t=35699  
https://hackaday.io/project/166144-retro-esp32  

Go-emu-launcher  
No ha funcionado.  
https://github.com/pelle7/odroid-go-emu-launcher  

Updater wifi  
Descarga aplicaciones de internet. Necesita un archivo con la lista de sitios.  
https://github.com/ripper121/odroidgoupdater  

## Otros proyectos  
https://github.com/32teeth  