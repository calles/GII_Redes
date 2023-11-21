## Instalar y configurar el servidor FTP en Windows Server 2019

Introducción
El protocolo de transferencia de archivos es un conjunto de reglas que definen cómo se pueden compartir (enviar y recibir) y manipular archivos (crear, renombrar y eliminar) a través de una red TCP/IP. 

### Paso 1: Iniciar el Administrador del servidor
Al igual que con todos los roles de Windows Server, tenemos que ir al Administrador del servidor para comenzar la instalación. Presione la tecla "Windows" y busque "Administrador del servidor" si aún no está abierto. Una vez abierto, haga clic en "Agregar roles y características".
![image](https://github.com/calles/GII_Redes/assets/22343642/f27bb1f1-6a63-4ed3-b567-a340b958388e)
![image](https://github.com/calles/GII_Redes/assets/22343642/47afb4f2-6969-4c10-b455-98d2295baf2f)

### Paso 2: Haga clic en Siguiente en el asistente
Paso 3: Seleccionar el tipo de instalación
En la página "Seleccionar tipo de instalación", seleccione "Instalación basada en roles o en funciones" y haga clic en "Siguiente"
![image](https://github.com/calles/GII_Redes/assets/22343642/4fbf43c3-1fbc-4188-ab3b-782c401499a4)

### Paso 4: Elegir el servidor de destino
Seleccione el servidor en el que instalará NFS y haga clic en "Siguiente"
![image](https://github.com/calles/GII_Redes/assets/22343642/c3d41229-e33b-4002-805a-2983f2eb20be)

### Paso 5: Seleccionar los roles que desea instalar
Seleccione la casilla de verificación "Servidor web (IIS)" y haga clic en "Agregar funciones" en la ventana emergente que aparecerá como se muestra a continuación. Haga clic en "Siguiente" una vez hecho esto.
![image](https://github.com/calles/GII_Redes/assets/22343642/642db7db-8579-4797-8a3e-b0d00f51af02)

### Paso 6: Seleccionar características
En la etapa "Seleccionar características", simplemente haga clic en "Siguiente" y haga clic en "Siguiente" nuevamente en la etapa "Rol de servidor web (IIS)" también.
![image](https://github.com/calles/GII_Redes/assets/22343642/45c5321c-908d-437a-b89d-7cb83c275de8)

### Paso 7: Seleccionar servicios de rol
Este es el paso que hemos estado esperando. Entre las muchas casillas de verificación, seleccione "Servidor de archivos" y presione "Siguiente". Después de eso, haga clic felizmente en "Instalar" y espere a que su servidor termine de instalarse.
![image](https://github.com/calles/GII_Redes/assets/22343642/b4a359ff-e784-4254-81d6-41046d5023c7)

Confirme las selecciones de instalación y presione "Instalar"
![image](https://github.com/calles/GII_Redes/assets/22343642/eb38b644-df4f-4591-8901-82c5920208a8)

### Paso 8: Configura tu FTP en modo pasivo
Configuremos ahora nuestro servidor FTP en modo pasivo como se describe en la sección de introducción.

Abra el Administrador del servidor >Herramientas > el Administrador de Internet Information Services (IIS)
![image](https://github.com/calles/GII_Redes/assets/22343642/d0ae1438-ee74-4447-b139-cc36ffdfd0b0)


Una vez abierto, proceda como se indica a continuación. Haga clic en el servidor para exponer el panel central.
![image](https://github.com/calles/GII_Redes/assets/22343642/ff97532a-43c1-49b0-8810-37242d36b092)


### Paso 9: Abrir la función
Seleccione "Compatibilidad con firewall FTP" y haga clic en "Abrir función" en el panel derecho como se ilustra. Alternativamente, puede hacer doble clic en "Soporte de firewall FTP". Eso abrirá una pequeña ventana emergente. Continúe con el paso 11.
![image](https://github.com/calles/GII_Redes/assets/22343642/7eda556a-ff77-48c7-afc7-b379928b0889)


### Paso 10: Compatibilidad con el cortafuegos FTP
Ingrese el rango de puertos para el modo pasivo en esta ventana emergente como se muestra a continuación y luego haga clic en "Aplicar" en el panel derecho.
![image](https://github.com/calles/GII_Redes/assets/22343642/7d16d312-b9b1-425c-b0f6-c41fac9d34b4)


Aparecerá la siguiente ventana emergente que le indicará que debe permitir el rango de puertos que configuramos en el firewall. Haga clic en "Aceptar". Después de eso, reinicie, FTP Server para realizar los cambios aplicados.

### Paso 11: Reiniciar el servidor FTP
Abra la aplicación de servicios, busque "Microsoft FTP Server", haga clic derecho sobre ella y seleccione reiniciar.
![image](https://github.com/calles/GII_Redes/assets/22343642/235f08e7-d804-4b17-8069-f455d66b06e9)

### Paso 12: Agregar los puertos en el Firewall
Uso Cómo abrir un puerto en el Firewall de Windows Server para agregar los puertos en su Firewall. Además, incluya el puerto 21. 
Debería verse como a continuación:
![image](https://github.com/calles/GII_Redes/assets/22343642/6ad5c8ff-4ae2-493d-b684-5ab94bedc648)


* Desde un cliente, conectarse al servidor FTP usando un cliente FTP como FileZilla o WinSCP. Para ello, introducir la dirección IP del servidor, el nombre de usuario y la contraseña.

* Transferir algunos archivos entre el cliente y el servidor usando el protocolo FTP. Por ejemplo, descargar archivo1.txt y archivo2.jpg del servidor al cliente, y subir archivo4.pdf y archivo5.docx del cliente al servidor.
