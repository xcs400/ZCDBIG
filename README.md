**Detecteur de passage à 0V**<br><br>
Montage avec composants trad. et pcb "simple face" maximalisé pour realisation home-made à la fraiseuse ou par gravure chimique<br>
Le projet Kicad complet est fourni<br>

![PCB](ZcdPcb.png)
![Schema](schematic.png)
![routage](routage.png)
![CNC](cnc.png)
relevé:
![scopeCNC](relevescope.png)

Ce montage a été integré dans mon router solaire pour commander la seconde voie utilisant le SSR.<br>
La premiere voie utilise le SSL commandé en PWM (la detection de passage a 0 est integré dans le SSL).

![SoloarRouter](IMG_6230.jpg)
![SoloarRouter](IMG_6231.jpg)
![SoloarRouter](IMG_6232.jpg)

Le logiciel de gestion est une version modifié de YARSOL . <br>
La modification consiste principalement en un module de communication directe vers Tuya ("wifi bidirectional meter") placé dans mon tableau electrique pour acceder à la consomation de la maison.
 ![tuya meter](tuyameter.jpg) <br>
Le rafraississement des informations de puissance se fait toutes les 3 secondes par wifi  (limite du module tuya), et ne necesssite pas l'utilisation de home assistant ou de serveur MQTT.   
