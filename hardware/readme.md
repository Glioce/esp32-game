### Esquemático  
https://github.com/hardkernel/ODROID-GO/blob/master/Documents/ODROID-GO_REV0.1_20180518.pdf  

Características técnicas de Odroid-Go  
https://wiki.odroid.com/odroid_go/odroid_go  

Otra consola basada en Odroid  
https://www.tindie.com/products/handheld-gaming/retro-esp32/  

Recompilar go-play  
https://forum.odroid.com/viewtopic.php?t=32081  

Datasheet PAM8304 monofónico  
https://www.diodes.com/assets/Datasheets/PAM8304.pdf  
Usaremos amplificador estéreo PAM8403  

### Bajar volumen
https://wiki.odroid.com/odroid_go/silent_volume

## LCD
Versión ISP  
http://www.lcdwiki.com/2.4inch_SPI_Module_ILI9341_SKU:MSP2402  
https://naylampmechatronics.com/blog/26_Tutorial-pantalla-TFT-t%C3%A1ctil-con-Arduino.html  

## Diferencias de módulos ESP32  
https://www.espressif.com/en/products/modules  
https://en.wikipedia.org/wiki/ESP32  

Datasheet  
https://www.espressif.com/sites/default/files/documentation/esp32-wrover_datasheet_en.pdf  

## Considerar mejoras en PCB
- Resistencia en serie con bocina. Volumen alto en entrada de amplificador con un poco de ruido. Todo se amplifica pero el ruido se percibe poco. Resistencia en bocina baja el volumen de todo, entonces el ruido se percibe menos.
- Headers a los lados para insertar TFT (sin headers para touch). ESP tiene que desplazarse, ¿dónde es mejor poner la antena?
- Recortar PCB hasta distancia de TFT
- Botones traseros quedan lejos de la tapa, se pueden poner extensiones. Conector USB también queda lejos ¿usar módulo extra?
- ¿Poner batería, cargador y chip UART?
- ¿ESP-32 Wrover-E es compatible?
- Imprimir nombres de pines en PCB
