### Práctica 3 (Router)

Utiliza el archivo dado por el profesor para terminar de configurar la red. Montar un servidor DHCP y agregar los ordenadores deben estar con IP dinámica.
Nota: todos los dispositivos tiene que hacer ping.

![image](https://github.com/calles/GII_Redes/assets/22343642/2c8fba11-012b-4aab-9c5b-6d6ce46c30c7)


[--> Archivo (packet tracer) <--](https://drive.google.com/file/d/1eUZzR4EBSQw8ppeGPmOSC4zZEI2FWmGz/view?usp=sharing)


### Sheet Cheat

#### Interfaz fa0/0:
- Router (config) # interface fa0/0
- Router (config-if) # ip address 192.168.1.1 255.255.255.0
- Router (config-if) # no shutdown
- Router (config-if) # exit

#### Interfaz fa0/1:
- Router (config) # interface fa0/1
- Router (config-if) # ip address 10.0.0.1 255.0.0.0
- Router (config-if) no shutdown
- Router (config-if) exit

#### Cambiar nombre del host
- Router> enable
- Router# configure terminal
- Router(config)# hostname R1

#### Contraseña parte 1
- R1(config)# line console 0
- R1(config-line)# password key1
- R1(config-line)# login
  
#### Contraseña parte 2
- R1(config)# enable secret key1

#### Ocultar contraseña
- R1(config)# service password-encryption

#### Banner
- R1(config)# banner motd #¡Acceso no autorizado únicamente!#

#### Reto:
Montar en ```Windows Server``` el servicio llamado DHCP para que asigne IP a un ordenador automaticamente y exponerlo en clases.
