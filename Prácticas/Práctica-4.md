# Práctica 4

Resuelve cada uno de los problemas para que la red funcione al 100%. El archivo será dado por el profesor.

![image](https://github.com/calles/GII_Redes/assets/22343642/cec2681c-4a01-4d3e-9cdb-8019001bf6cb)

[-->Descarga el archivo<--](https://drive.google.com/file/d/1xQGGHGWL1XLhQVPdJ_ynsQW2u_dop2Iv/view?usp=sharing)

Actividad:

1. Todos los host de la red "A" tienen que acceder al Web Server.
2. El host 126.4.32.3 no puede acceder al TFTP Server por FTP.
3. El host IP 126.0.0.2 y 126.0.0.3 no puede hacer ping al DATA Server.
4. Habilitar en el DHCP del servidor DHCP Server for VLANs para red "J"
5. Agregar un router y un pc y conectarlos con el router 18 para que el pc 14 pueda hacer ping.

## Pista número 1:

```ENABLE```
```CONFIG TERMINAL ```
```IP ROUTE [red destino] [mascara de red] [interfaz de salida] ```

Ej: ip route 193.0.0.0 255.255.0.0 Serial0/0/0
