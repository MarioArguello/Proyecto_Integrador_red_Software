# Proyecto_Integrador
Red_Urb_la_laguna
Descripción:
Los estudiantes deberán formar grupos de 4 para diseñar la red de una etapa de una urbanización de acuerdo a las siguientes indicaciones:
Cada grupo deberá escoger una urbanización (mediante google maps) y una dirección de red de clase B, y postearla en el foro para evitar    temas repetidos. Luego en base al número de casas y manzanas realizar un adecuado direccionamiento de red que evite que el broadcast de una manzana afecte a otra (subredes y vlans).
Finalmente realizar una simulación de la red en packet tracer, representando cada manzana con 4 pcs e interconectándolas entre sí mediante los dispositivos de red respectivos. Toda la etapa debe salir a internet mediante una única conexión.


#Manuaal de implementacion

Red diseñada

![red](https://user-images.githubusercontent.com/60244917/75213417-07ee0780-5758-11ea-85ac-ccde9826bd8f.PNG)




Las redes se nombran como:

La red 1 tiene 4 PC.

La red 2 tiene 6 PC.

La red 3 tiene 4 PC.

La red 4 tiene 4 PC.

La red 5 tiene 4 PC.

La red 6 tiene 5 PC.

La red 7 tiene 4 PC.

La red 8 tiene 4 PC.

La red 9 tiene 5 PC.


Cada  manzana tiene asignada una red, todos los switch estan conectados con un switch de capa 3,la asignacion de ip fue la siguiente:

red 1: 170.100.1.1/ 255.255.255.224

red 2: 170.100.2.1/ 255.255.255.224

red 3: 170.100.3.1/ 255.255.255.224

red 4: 170.100.4.1/ 255.255.255.240

red 5: 170.100.5.1/ 255.255.255.240

red 6: 170.100.6.1/ 255.255.255.192

red 7: 170.100.7.1/ 255.255.255.240

red 8: 170.100.8.1/ 255.255.255.240

red 9: 170.100.9.1/ 255.255.255.192


Cada red tiene las vlans asignadas a todos los puertos de las pc:

red 1: vlan 50, f0/3 - 6

red 2: vlan 60, f0/2 - 8

red 3: vlan 69, f0/2 - 6

red 4: vlan 32, f0/2 - 7

red 5: vlan 47, f0/2 - 7

red 6: vlan 56, f0/2 - 8

red 7: vlan 94, f0/2 - 7

red 8: vlan 78, f0/2 - 8

