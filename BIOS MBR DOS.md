# BIOS MBR DOS  

**Antiguo:** El tamaño máximo de partición son **2TB.**  
**Nuevo:** UEFI-GPT El tamaño máximo de partición no existe prácticamente, ya que es un número altísimo concretamente un **máximo** de 18 exabytes (~**18,8 millones de terabytes**) de espacio.  

**LAS REGLAS SON LAS SIGUIENTES**  
  
* Máximo 4 particiones primarias
* 1 de las primarias debe ser extended 
* Dentro de la extended puede haber **"n logicas"**
* Y la última norma, la primaria debe ser "Active"  
---> Una extended no puede ser "Active" <---  
  * **LINUX** da igual el orden, ellos se entienden entre ellos.
  * **WINDOWS** Necesita una primaria activa ya que se ejecuta el bootmanager.
  * **IMPORTANTE** La partición primaria activa del bootmanager no tiene porque ser de 100MB, se puede instalar Windows en la misma partición.  
  BOOTMGR - WINDOWS
  LINUX - GRUB
# **MBR TO GPT
* Para poder cambiar a modo **MBR** se tiene que entrar en la BIOS y allí dentro cambiar a modo Legacy y si queremos poner GPT cambiamos a modo UEFI.  
![alt text](https://www.solvetic.com/uploads/monthly_05_2017/tutorials-9832-0-68952600-1495445584.png)
