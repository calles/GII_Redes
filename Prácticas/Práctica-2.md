### Práctica 2 (Switch)

#### Ejercio para alumnos con carné terminados en número "PAR"

1. En un **Hotel** de 3 plantas, se necesita crear una red LAN (Topologia de red en árbol).
2. Las plantas son (Sala de juegos [planta -1] , Hall [Planta 0] y Habitaciones [Planta 1]).
3. Para cada planta se necesita asignar 4 portátiles con sus respectivos nombres (Hostname) y sus propias IPs correspondiente al sitio.
4. Configurar un switch (nombre y seguridad) por cada planta.
5. Los nombres dependerán de cada planta y del área en el que se encuentren.
6. En un 4º switch configurar las Vlans para la red: Machines, Hall, Rooms.
7. Desabilitar los puestos que no se esten utilizando.
8. Hacer pruebas de ping para garantizar que las redes esten aisladas.
9. Agregar un servidor que este conectado al 4º switch.

+ NOTA: Cada planta dispone de un cuarto de comunicaciones para guardar los dispositivos de red. explicar en una nota la seguridad física para entrar a los cuartos de comunicaciones.

#### Ejercio para alumnos con carné terminados en número "IMPAR"

1. En un **Centro Comercial** que posee 3 áreas en fila, se necesita crear una red LAN (Topologia de red en estrella extendida).
2. Las áreas son: (Joyería [bloque 1], Atención al cliente [bloque 2] y Perfumeria [bloque 3]).
3. Para cada negocio se necesita asignar 4 ordenadores con sus respectivos nombres (Hostname) y sus propias IPs correspondiente al sitio.
4. Configurar un switch (nombre y seguridad) por cada área.
5. Los nombres dependerán de cada planta y del área en el que se encuentren.
6. Habilitar en el switch que estará en Atención al cliente las Vlans para la red: Jewelry, Perfume, Support.
7. Desabilitar los puestos que no se esten utilizando.
8. Hacer pruebas de ping para garantizar que las redes esten aisladas.
9. Agregar un servidor que este conectado al switch que estará en Atención al cliente.

+ NOTA: Cada planta dispone de un cuarto de comunicaciones para guardar los dispositivos de red. explicar en una nota la seguridad física para entrar a los cuartos de comunicaciones.


## Cheat Sheet

### Desabilitar puertos de switch

```Switch>enable``` <br/>
```Switch#configure terminal``` <br/>
```Switch(config)#interface range fastEthernet 0/3-9``` <br/>
```Switch(config-if-range)#shutdown```

### Cambiar nombre al switch

```Switch>enable``` <br/>
```Switch#configure terminal``` <br/>
```Switch(config)#hostname Xbox``` <br/>
```Xbox(config)#```

### Colocar seguridad al switch

```Switch>enable``` <br/>
```Switch#configure terminal``` <br/>
```Switch(config)#line console 0``` <br/>
```Switch(config-line)#password key1``` <br/>
```Switch(config-line)#login``` <br/>
```Switch(config)#exit``` <br/>
```Switch#exit``` <br/>

```Switch>enable``` <br/>
```Switch#configure terminal``` <br/>
```Switch(config)#enable secret key2``` <br/>
```Switch(config)#exit``` <br/>
```Switch#exit```

### Colocar un banner de bienvenida

```Switch>enable``` <br/>
```Switch#configure terminal``` <br/>
```banner motd #ACCESO NO AUTORIZADO, NO ENTRAR#``` <br/>
```Switch(config)#exit``` <br/>
```Switch#exit```

### Configuración IP a la Vlan

```Switch>enable``` <br/>
```Switch#configure terminal``` <br/>
```interface vlan 1``` <br/>
```ip address (Dirección IP – Máscara de subred)``` <br/>
```no shutdown```

### Guardar en memoria

```copy running-config startup-config```

### Nombre para las VLan

```Switch>enable``` <br/>
```Switch#configure terminal``` <br/>
```vlan 1``` <br/>
```name Practica2``` <br/>
```exit```

### Consultar puestos y vlans

```Switch#show vlan brief``` <br/>
o <br/>
```Switch#show vlan name practica2```

### Cambiar Vlan
```Switch>enable``` <br/>
```Switch#configure terminal``` <br/>
```interface fastEthernet 0/1``` <br/>
```switch access vlan 10``` 

### Comandos de Cisco

```show ?```
