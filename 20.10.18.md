# MBR
El **(MBR)** Registro Principal de Arranque es un sector de **512 bytes** al princio del disco duro que gracias a su inicialización de comandos a iniciar el Pc es el que se encarga de cargar el sistema operativo. Contiene un programa ejecutable en el primer registro del disco y una tabla donde están definidas las particiones del disco.  
Tiene 3 componentes.  
* Información primaria del bootloader en sus primeros 446 bytes.  
* Información de la tabla de partición en los siguientes 46 bytes.  
* Revisión de validación del (MBR) en los últimos 2 bytes.  
