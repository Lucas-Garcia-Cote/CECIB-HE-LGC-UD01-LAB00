## 1 ¿Por qué DC-1 no debe tener adaptador NAT ni puente?

Porque es una máquina que sabemos que no es segura, por lo que debemos aislarla de la red de nuestro ordenador para que no se vea comprometido

## ¿Para qué sirve el servidor DHCP que creaste en H3?

Para por así decirlo "delimitar" la zona donde se encuantran las dos máquinas dentro de labnet, ya que al crear una red interna no delimitamos las ip de las máquinas, asique creamos el DHCP para ello

## Qué hacen "netdiscover" y "ping", y qué información te dio cada uno?

"netdiscover" es un comando que se utiliza para ver todos los dispositivos que hay en una red, sin incluir a la máquina que ejecuta el comando, mientras que "ping" es una prueba que se hace para ver si hay conectividad entre las dos máquinas

---
---
---

## Bitácora de IA

Tuve un problema que consistía en que el kali solo me cogia la ip de uno de los DHCP, y nunca los dos al mismo tiempo, por lo que le pregunté a la IA cual era el comando para que kali pidiera ip a los DHCP, porque no lo recordaba. Al final lo resolví usando "sudo apt install isc-dhcp-client" para instalar un servicio que me permitía utilizar el comando "sudo dhclient -v eth0" para que pidiera una ip para el puerto que no la tenía