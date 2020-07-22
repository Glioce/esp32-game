## Mini joystick XKB-Enterprise-TM-2027  
https://lcsc.com/product-detail/Multi-Directional-Switches_XKB-Enterprise-TM-2027_C318948.html  
https://datasheet.lcsc.com/szlcsc/2002271736_XKB-Enterprise-TM-2027_C318948.pdf  
Se creó el componente en Fusion 360 (símbolo y footprint)

Otros mini joysticks  
ALPS SKRHABE010 Se conecta en "diagonal"
https://www.mikroe.com/blog/a-smart-navigation-key-concept

Footprint anterior compatible con SF303GJ26  
https://www.sparkfun.com/datasheets/Components/Buttons/SF303GJ26-3.pdf  
https://www.mouser.mx/datasheet/2/15/SKRH-1370966.pdf  
https://lcsc.com/product-detail/5-way-Tactile-Switches_ALPS-Electric-SKRHABE010_C139794.html  

SparkFun-Switches.lbr contiene SF303GJ26  
https://github.com/sparkfun/SparkFun-Eagle-Libraries  

otros formatos  
https://componentsearchengine.com/part/2856952/model/download  

## ESP32 WROVER  
Se utilizó versión de 32teeth  
https://github.com/32teeth/Eagle-Libraries-by-32teeth/tree/master/lbr  

## Push button tactile 2pin  
https://www.diymodules.org/eagle-show-library?type=usr&id=2105&part=switch-tact.lbr  
No es la medida exacta, las terminales deben tener distancia entre centros de 0.2 in.  

Se cambiarán por botones de 4 pines con vástago largo.  

## Conector Micro USB B  
https://en.wikipedia.org/wiki/USB  

Through hole  
https://github.com/snakeye/eagle-lib/tree/master/connectors  
https://www.diymodules.org/eagle-show-object?type=usr&id=1012211711&device=ZX62D-B-5PA8  
https://www.diymodules.org/eagle-show-object?type=usr&id=1012211141&device=ZX62D-B-5P8  

SMD  
https://github.com/dvdnhm/Maker-Tools-Eagle-Libraries  

Podría tomarse de aquí  
https://github.com/adafruit/Adafruit-Pro-Trinket-PCBs  

## Tutoriales  
Crear componentes electrónicos en Fusion 360  
https://www.youtube.com/watch?v=zqar0XWtFaY  

Descripción de las capas en Eagle  
https://www.autodesk.com/products/eagle/blog/every-layer-explained-autodesk-eagle/  

Llenar espacio vacío de PCB con cobre  
https://www.autodesk.com/products/eagle/blog/design-rule-check-pcb-layout-basics-3/

## Notas  
Al parecer hay un bug en F360. La capa "solder mask" ignora los pads de componentes SMD  
https://forums.autodesk.com/t5/fusion-360-electronics/solder-mask-in-3d-pcb-ignores-tstop-and-bstop/td-p/9477740  
Se puede solucionar importando el diseño en Eagle  

Para exportar PDF desde F360 escribir `PRINT` en la barra de comandos.  
