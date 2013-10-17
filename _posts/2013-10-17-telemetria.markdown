---
layout: post
title:  "Telemetria"
date:   2013-10-17 12:45:21
categories: tecnologia
---

Mediante la **telemetría** es posible poder medir, ver y operar distintos dispositivos de manera remota, almacenar información, etc.

Existe multitud de tecnologías pensadas para la infinidad de propósitos que requieren una infraestructura de este tipo, veamos un poco algunas de ellas.

**Inalámbrica**

Como dice el nombre, sin cables, esto reduce a cualquier sistema que utilice ondas de radio para transmitir la informacion. La mayoría de estas implementaciones son de uso contidiano, en teléfonos celulares, 
notebooks... 

- Red GSM
- Red 3g
- WiFi
- WiMax
- Packet Radio
- Onda Corta

**Cableada**

Y en menor medida podemos utilizar otros tipos de accesos al medio, caso mas raro, dado que en la mayoría de las veces que se precisa hacer uso de la telemetría es en casos que el dispositivo esta en un lugar de 
difícil acceso, o que no haya disponibilidad de redes o sistemas de comunicación y transporte cómodos.
Estas formas utilizan normalmente sistemas cableados, con puntos lo suficientemete distantes para que hacer que sea una inversion costosa de implementar y mantener, aunque a la vez se puede decir que es mas "fiable".


- Red UTP</li>
- Fibra Óptica</li>
- Red Telefónica</li>

----------


####Implementación

El diseño de una estructura está absolutamente determinada por las condiciones que presenta el caso, difícilmente una necesidad es igual a otra, por lo tanto es complicado plantear generalidades, pero vamos a hacer el 
intento.

**Medio Ambiente**

Supongamos que tenemos un dispositivo que mide la temperatura ambiente de un lugar, y nosotros necesitamos ver esa temperatura en nuestra computadora que esta a 500Km del lugar de medición, para ello necesitamos:

- Dispositivo de medición
- Unidad de telemetría
- Servidor de datos
- Cliente de datos

En este modelo que creo se autoexplica, el termómetro mide temperatura, por una salida envia los datos al dispositivo de telemetría, este a su vez reenvia esos datos a un servidor de bases de datos, y luego el 
observador con un programa se conecta a la base de datos y puede ver que temperatura hace a 500Km de su oficina.


####Desarrollo

Además de poder transportar datos a lugares remotos, muchas veces es necesario procesarlos, graficarlos, etc. Nuestro equipo de desarrollo junto con el cliente se encarga de desarrollar el software de interpretacion de 
datos si es necesario, ademas de cualquier servicio asociado.
