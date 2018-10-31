# ¿Como cambiar la password de root?  
**[Pasos si sabemos la contraseña]**
- Abrimos el terminal  
- Escribimos el comando **# sudo passwd root** y nos pedirá la contraseña de nuestro usuario.  
- Cuando hayamos puesto nuestro usuario nos pedira una **nueva password**, la ponemos y nos pedira que la volvamos a **repetir**.  
En esta imagen lo podemos ver:  

![alt text](https://image.ibb.co/jzx7a0/screenshot-from-2013-07-20-192632.png)  


**[Pasos si no sabemos la contraseña]**  
- Inicimos el PC y mantenemos pulsamos la tecla **SHIFT**, lo que hará que se muestre el menú **GRUB o de arranque.**  
  ![alt text](https://image.ibb.co/b7Qca0/recuperar-la-contrasec3b1a-de-linux-usando-grub.png)  
  
- Una vez dentro, pulsaremos la tecla de desplazamiento inferior hasta posicionarnos sobre la opción **“recovery mode”** y puslaremos ENTER.  
- Ahora escribimos los siguientes comandos.  
- Este comando nos dará permisos de escritura y lectura.  **mount -rw -o remount /**
- Siguiente comando: **passwd nombreusuario** donde nombre de usuario es el nombre que tiene tu cuenta.
- Ahora te pedirá que crees una nueva contraseña de UNIX nueva, escribela y confirma con ENTER.
  Ejemplo con una imagen:  
  
  ![alt text](https://image.ibb.co/gfHOF0/cambiar-password-root.jpg)
