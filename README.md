# esp32-game

Se probaron 2 bootloaders: Odroid-Go y Esplay-Micro.  

**Esplay-Micro**  
Ventajas:  
+ Tiene más botones por lo que algunos juegos son más fáciles de usar (ej. Doom)  
+ Funciona en ESP32 con flash de 4MB  

Desventajas:  
+ Ocupa más pines para la tarjeta SD y para la salida de audio  
+ La salida de audio es digital, por lo que se necesita un DAC externo  
+ Los botones necesitan un módulo I2C externo  

**Odroid-Go**  
Ventajas:  
+ Utiliza pocos módulos externos (pantalla SPI, lector de SD, y amplificador de audio opcional)  
+ La pantalla y la SD comparten 3 pines SPI, se ahorran pines (la descripción de Esplay dice que esto puede causar problemas, pero hasta ahora no se han presentado)  
+ Salida de audio analógico directo del ESP32  
+ Tiene varios ports de juegos y launchers de emuladores  

Desventajas  
+ Necesita ESP32 con flash de al menos 8MB  

Se eligió Odroid-Go porque utiliza pocos componentes electrónicos.  

## Organización
La carpeta "hardware" contiene información de los dispositivos electrónicos probados y los diseños personalizados.  

La carpeta "software" contiene información del software instalado en el esp-32.  

La carpeta xtra tiene recusos interesantes, pero que no son necesarios en el estado final del proyecto.  
