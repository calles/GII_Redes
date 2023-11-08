### Práctica 2 (Switch)

#### Ejercio para alumnos con carné terminados en número "PAR"

1. En un **Hotel** de 3 plantas, se necesita crear una red LAN (Topologia de red en árbol).
2. Las plantas son (Sala de juegos [planta -1] , Hall [Planta 0] y Habitaciones [Planta 1]).
3. Para cada planta se necesita asignar 4 portátiles con sus respectivos nombres (Hostname) y sus propias IPs de acuerdo al sitio.
4. Configurar un switch (nombre y seguridad) por cada planta.
5. Los nombres dependerán de cada planta y del área en el que se encuentren.
6. En un 4º switch configurar las Vlans para la red: Machines, Hall, Rooms.
7. Desabilitar los puestos que no se esten utilizando.
8. Hacer pruebas de ping para garantizar que las redes esten aisladas.
9. Agregar un servidor que este conectado al switch de la planta 0. (No el 4º switch)

+ NOTA: Cada planta dispone de un cuarto de comunicaciones para guardar los dispositivos de red. explicar en una nota la seguridad física para entrar a los cuartos de comunicaciones.

#### Ejercio para alumnos con carné terminados en número "IMPAR"

1. En un **Centro Comercial** que posee 3 áreas en fila, se necesita crear una red LAN (Topologia de red en estrelle extendida).
2. Las áreas son: (Joyería [bloque 1], Atención al cliente [bloque 2] y Perfumeria [bloque 3]).
3. Para cada negocio se necesita asignar 4 ordenadores con sus respectivos nombres (Hostname) y sus propias IPs de acuerdo al sitio.
4. Configurar un switch (nombre y seguridad) por cada área.
5. Los nombres dependerán de cada planta y del área en el que se encuentren.
6. Habilitar en el switch que estará en Atención al cliente las Vlans para la red: Jewelry, Perfume, Support.
7. Desabilitar los puestos que no se esten utilizando.
8. Hacer pruebas de ping para garantizar que las redes esten aisladas.
9. Agregar un servidor que este conectado al switch que estará en Atención al cliente.

+ NOTA: Cada planta dispone de un cuarto de comunicaciones para guardar los dispositivos de red. explicar en una nota la seguridad física para entrar a los cuartos de comunicaciones.


## Cheat Sheet

### Desabilitar puertos de switch

``Switch>enable``
``Switch#configure terminal``
``Switch(config)#interface range fastEthernet 0/3-9``
``Switch(config-if-range)#shutdown``
