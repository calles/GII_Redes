# GII_Redes
`Contacto: **rodrigo.zaldana.calles@uneatlantico.es**`
_________
- [X] 1. [**Introducción**](https://docs.google.com/presentation/d/1yr5lPUGB0K5CXoYkVqf3hYfCPm9T3z6tUipzuGNCgBI/edit?usp=sharing)
- [X] 2. [Azure](https://azure.microsoft.com/en-us/free/students/) + [Packet Tracert](https://www.netacad.com/courses/packet-tracer)
- [ ] 3. [**C. Física**](https://github.com/calles/GII_Redes/blob/main/README.md#la-capa-f%C3%ADsica)
- [ ] 4. [Práctica 1 (Topologías - PacketT)](https://github.com/calles/GII_Redes/blob/main/Pr%C3%A1cticas/Practica-0.md)
- [ ] 5. **C. Enlace de datos**
- [ ] 6. Práctica 2 (Config. Switch - PacketT)
- [ ] 7. **C. Red**
- [ ] 8. Práctica 3 (Config. Router - PacketT)
- [ ] 9. **C. Transporte**
- [ ] 10. Práctica 4 (Config. Servidor FTP VS TFTP - Azure)
- [ ] 11. _PARCIAL (C. 1-5)_
- [ ] 12. **C. Sesión**
- [ ] 13. Práctica 5 (Config. Servidor NFS - Azure)
- [ ] 14. **C. Presentación**
- [ ] 15. Práctica 6 (Certificado SSL - Azure)
- [ ] 16. **C. Aplicación**

## Modelo OSI
El Modelo OSI fue creado por la ISO (Organización Internacional de estándares).

Se utiliza para el diseño de redes de datos, especificaciones de funcionamiento y resolución de problemas.
En un principio, OSI pretendía sentar unas reglas que definieran un marco de actuación para el conjunto de protocolos que lo formaban.

Lamentablemente , Internet basado en TCP/IP fue adoptado velozmente y el modelo OSI quedó atrás.
No obstante aún permanece como una guía universalmente aceptada , ya que define con precisión las actividades en cada capa.

El sucesor, el modelo TCP/IP, define cuatro categorías de funciones que deben tener lugar para que las comunicaciones sean exitosas. La arquitectura de la suite de protocolos TCP/IP sigue la estructura de este modelo. Por esto, es común que al modelo de Internet se lo conozca como modelo TCP/IP.

![image0](https://github.com/calles/GII_Redes/assets/22343642/60b6ae2f-0b27-4609-a38b-068dc64d3642)

## La Capa Física
La Capa Física es la primera capa del Modelo OSI (Open Systems Interconnection) y se encarga de gestionar la comunicación física entre los dispositivos de una red. 
Esta capa se encarga de la transmisión de bits a través del medio de comunicación físico, como cables o señales inalámbricas, y establece las características técnicas necesarias para que los datos puedan fluir de un dispositivo a otro.

En la Capa Física se definen diferentes aspectos relacionados con la transmisión de bits, como la codificación de la señal, la velocidad de transmisión, el tipo de cableado utilizado y la topología de la red. 
Además, esta capa también se encarga de gestionar la sincronización de los dispositivos y de detectar y corregir posibles errores de transmisión.

Es importante destacar que la Capa Física es independiente del tipo de red o del protocolo de comunicación utilizado. 
Su función principal es asegurar que los bits puedan ser transmitidos de manera fiable y eficiente a través del medio físico, para que las capas superiores del Modelo OSI puedan encargarse de la transferencia de datos de manera correcta.


1. ¿Cuál de las siguientes es una característica del cable de fibra óptica monomodo?
- [ ] generalmente utiliza LED como fuente de luz
- [ ] núcleo relativamente mayor con varias rutas de luz
- [ ] menos costoso que el multimodo
- [ ] generalmente utiliza láseres como fuente de luz
 
2. ¿Cuáles son las tres medidas para la transferencia de datos? (Elija tres).
- [ ] capacidad de transferencia útil
- [ ] frecuencia
- [ ] amplitud
- [ ] rendimiento– crosstalk
- [ ] ancho de banda
 
3. ¿Qué característica del cable UTP ayuda a disminuir los efectos de la interferencia?
- [ ] el trenzado metálico del blindaje
- [ ] el revestimiento reflectante alrededor del núcleo
- [ ] el trenzado de los hilos en el cable
- [ ] la protección del material en el revestimiento exterior
 
4. ¿Cuáles son las características que describen al cable de fibra óptica? (Elija dos).
- [ ] No lo afectan la EMI (Interferencia electromagnética) ni la RFI (Interferencia de radiofrecuencia).
- [ ] Cada par de cables se encuentra envuelto en papel metálico.
- [ ] Combina la técnicas de cancelación, blindaje y trenzado para proteger los datos.
- [ ] Cuenta con una velocidad de 100 Mbps.
- [ ] Es el tipo de cableado LAN más costoso.
 
5. ¿Cuál de las siguientes opciones se considera un beneficio de lo inalámbrico como elección de medios?
- [ ] mayor movilidad del host– menos riesgos de seguridad
- [ ] reducida susceptibilidad a la interferencia
- [ ] menor impacto del entorno sobre el área de cobertura efectiva
 
6. ¿Qué método de transmisión de señal utilizan las ondas de radio para transportar señales?
- [ ] eléctrico
- [ ] óptico
- [ ] inalámbrico
- [ ] acústico

Referencias:
https://tododeredes.com/modelo-osi/capa-1/
