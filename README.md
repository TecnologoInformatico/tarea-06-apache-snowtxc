# apache

Reemplace `$ALUMNO` por el nombre de su nombre de usuario en www.tecnologoinformatico.com

EJ: `dmascheroni`

1. Cree el directorio ~/repositorios y dentro clone el
repositorio: `https://github.com/TecnologoInformatico/AdmInf-web.git`
2. Actualice el repositorio de la lista de paquetes.
    `apt update`
3. Instalar el servidor Apache mediante apt.
4. Cree el directorio /var/www/$ALUMNO
5. Asigne como propietario del directorio su usuario.
6. Configure un nuevo Virtual host. (copiando el archivo de configuración por defecto)
  6.1. ServerName $ALUMNO.tecnologoinformatico.com
  6.2. Correo de contacto con el administrador.
  6.3. El root de la aplicación. (/var/www/$ALUMNO)
7. Modifique el archivo /etc/hosts de modo que el ServerName coincida con este equipo `127.0.0.1`.
8. Reinicie el servidor apache para que los cambios tengan efecto.
9. Copie el contenido del directorio ~/repositorios/AdmInf-web a /var/www/$ALUMNO, de tal modo que el contenido del repositorio antes clonado se encuentre en el root de la aplicación.
10. Verifique que el servidor funcione correctamente.
11. Ingrese la IP del servidor y el servername a continuación:

```json
{
    "serverName": "",
    "ip": ""
}
```


## Solucion

1.
   generar y agregar la clave ssh publica al la instancia en oracle

2. contectarse al servidor publicando la clave publica ssh
<br>
<code>
   ssh -i rsa_pub ubuntu@ip 
</code> 

3. clono el repositorio
<br>
<code>
   mkdir repositorios
</code> 
<br>
<code>
   git clone https://github.com/TecnologoInformatico/AdmInf-web.git
</code> 

4. instalacion de apache
<br>
<code>
   sudo apt install apache2
</code> 
<br>

5. crear directorio
<br>
<code>
    sudo mkdir  /var/www/ALUMNO
</code> 
<br>


6. asignar permisos
<br>
<code>
    sudo  chmod 777 ALUMNO/
</code> 
<br>

7. asignar propietario
<br>
<code>
    sudo chown ubuntu ALUMNO/
</code> 
<br>



