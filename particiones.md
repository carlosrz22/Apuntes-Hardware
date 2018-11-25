# ¿Que es una partición?  
Una partición es el nombre que se le da a cada división presente en una sola unidad física de almacenamiento de datos. Para que se entienda, **tener varias particiones es como tener varios discos duros en un solo disco duro físico**, cada uno con su **sistema de archivos** y funcionando de manera diferente.  

![alt text](http://www.ite.educacion.es/formacion/materiales/43/cd/modulo_2/quitar06.png)

# ¿Que es un sistema de archivos?  
El sistema de archivos es un componente del sistema operativo que se encarga de administrar la memoria de cada unidad. Se encarga de **asignarle a los archivos el espacio que necesiten**, ordenarlos, permitir el acceso a ellos y administrar el espacio libre de las unidades de almacenamiento.  
**Cada sistema de archivos tiene sus propias ventajas y limitaciones**, por lo que es importante conocerlos para elegir el que mejor se ajusta a cada necesidad que tengas.  
Para crear un sistema de archivos dentro de nuestra partición lo aremos con **mkfs**  

![alt text](https://i.ibb.co/9nv6f93/sistema-de-archivos-Particiones.png)

Tenemos diferentes sistemas de archivos:  
- **FAT 32** Es un tipo de sistema de archivos FAT. El tamaño máximo de un archivo en FAT32 es de **4 gigabytes**.
- **NTFS** Tiene más permisos y configuraciones de seguridad que FAT 32. Además no tiene un límite de tamaño de archivos.

Después de haber terminado de hacer las particiones tendremos que utilizar el **partprobe** és un comando que nos lee el disco duro y que reconoze las particiones, si no tendremos que reiniciar el ordenador y seria una perdida de tiempo.

Con el **partprobe** és el método que tenemos que utilizar siempre y que será útil.
Pero tenemos un **apaño** que si por una razón u otra no nos va el **partprobe** tenemos el:

**Kpartx -a "disco"**

Y nos quedará guardado en **mapper** y para entrar deberemos de hacer **ls "disco"/mapper/"disco". 

# Comandos Particiones

**a**  Partición boot

**n**  Creamos partición

**l**  Partición lógica

**p**  Partición primaria 

**e**  Partición extendida

**t**  Cambiamos tipo 

**82** Swap

**7**  Ntfs
