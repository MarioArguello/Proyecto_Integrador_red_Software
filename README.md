# Proyecto_Integrador
Red_Urb_la_laguna
Proyecto Integrador

Planteamiento del problema
Los estudiantes deberán formar grupos de 4 para diseñar la red de una etapa de una urbanización de acuerdo a las siguientes indicaciones: Cada grupo deberá escoger una urbanización (mediante google maps) y una dirección de red de clase B, y postearla en el foro para evitar temas repetidos. Luego en base al número de casas y manzanas realizar un adecuado direccionamiento de red que evite que el broadcast de una manzana afecte a otra (subredes y vlans). Finalmente realizar una simulación de la red en packet tracer, representando cada manzana con 4 pcs e interconectándolas entre sí mediante los dispositivos de red respectivos. Toda la etapa debe salir a internet mediante una única conexión.
La  urbanizacion elegida fue la Laguna
link del lugar :  https://www.google.com/maps/place/Urb.+La+Laguna,+Samborond%C3%B3n/@-2.0746294,-79.8769288,391m/data=!3m1!1e3!4m5!3m4!1s0x902d12fe6d24617f:0xcf125f461c63382e!8m2!3d-2.0772269!4d-79.8765835


![mapa](https://user-images.githubusercontent.com/60244917/75835823-f4612300-5d8d-11ea-8330-cba87399496a.PNG)

Red diseñada
 
 
![final](https://user-images.githubusercontent.com/60244917/75836287-6b4aeb80-5d8f-11ea-9255-e40aa53d6b94.jpg)
 
 
Justificación

Se utilizó la urbanización “La Laguna” para el diseño de la red, en la cual consta de 9 redes a cada una se le asignó una vlan diferente y estas se conectan en una única conexión para salir a internet.
Acontinuación se indica cuantos dispositivos tiene asignado cada red de la urbanización:
 	La red 1 tiene 4 PC.
 	La red 2 tiene 6 PC.
 	La red 3 tiene 4 PC.
 	La red 4 tiene 4 PC.
 	La red 5 tiene 4 PC.
 	La red 6 tiene 5 PC.
 	La red 7 tiene 4 PC.
 	La red 8 tiene 4 PC.
 	La red 9 tiene 5 PC.

Además cada manzana tiene asignada una red y todos los switch están conectados con un switch de capa 3. La asignación de ip a cada red fue la siguiente:

 	red 1: 170.100.1.1/ 255.255.255.224
 	red 2: 170.100.2.1/ 255.255.255.224
 	red 3: 170.100.3.1/ 255.255.255.224
 	red 4: 170.100.4.1/ 255.255.255.240
 	red 5: 170.100.5.1/ 255.255.255.240
 	red 6: 170.100.6.1/ 255.255.255.192
 	red 7: 170.100.7.1/ 255.255.255.240
 	red 8: 170.100.8.1/ 255.255.255.240
 	red 9: 170.100.9.1/ 255.255.255.192

Se agregó vlans diferentes para la seguridad de los usuarios e hicimos la red segura asignando vlans diferentes a los puertos ocupados y libres para que las personas exteriores no obtengan acceso a la red. La configuración de vlans para cada red fue la siguiente:
 	red 1: vlan 50, f0/3 - 6
 	red 2: vlan 60, f0/2 - 7
 	red 3: vlan 69, f0/2 - 5
 	red 4: vlan 32, f0/2 - 5
 	red 5: vlan 47, f0/2 - 5
 	red 6: vlan 56, f0/2 - 6
 	red 7: vlan 94, f0/2 - 5
 	red 8: vlan 78, f0/2 – 5
 	red 9: vlan 68, f0/2 – 5
Ninguna vlan 1 tiene configurada la dirección IP pero las demas vlans si se les asignó una IP la cual se detalla en la siguiente tabla:

Switch	VLAN	IP
Red 1	50	170.100.1.1/27
Red 2	60	170.100.2.1/27
Red 3	69	170.100.4.1/27
Red 4	32	170.100.4.1/28
Red 5	47	170.100.5.1/28
Red 6	56	170.100.6.1/26
Red 7	94	170.100.7.1/28
Red 8	78	170.100.8.1/26
Red 9	68	170.100.9.1/26

Todos los puertos troncales fueron asignados al puerto 1 de cada red, además se configuró las vlans nativas para poder tener control de todas las redes.
Una vlan nativa está asignada a un puerto troncal. Los puertos de enlace troncal son los enlaces entre switches que admiten la transmisión de tráfico asociado a más de una vlan. Los puertos de enlace troncal admiten el tráfico proveniente de muchas vlan (tráfico con etiquetas), así como el tráfico que no proviene de una vlan (tráfico sin etiquetar).

Restricciones
Se realizó la simulación de la topología en Cisco Packet Tracer versión 7.3 para el diseño de la red ya que es de fácil utilización y nos permite analizar el contenido de los paquetes para poder corregir posibles errores al simular la conectividad.
Para realizar correctamente la simulación de la red se siguió los siguientes lineamientos:
1.	Se usó switch de diseño 2960-24TT
2.	Se usó PC genéricos.
3.	Se utilizó cables de conexión directa para toda la red.
4.	Se asignó IP estática a todas las PC de la red.
5.	Se configuro 9 vlans para cada manzana de la urbanización.

