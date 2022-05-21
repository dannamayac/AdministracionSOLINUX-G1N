Creación del archivo README.md

Taller 7

1. Se instala en la base de datos de la maquina virtual mariadb usando el comando sudo dnf install maria db-server-y

<img src= "https://github.com/dannamayac/AdministracionSOLINUX-G1N/blob/main/InfraestructuraComputacional/Seguimiento/7/1%20(1).jpgg" style="max-width:100%;">

2. Se inicia el servicio de la base de datos mediante el comando systemctl star maria db

<img src= "https://github.com/dannamayac/AdministracionSOLINUX-G1N/blob/main/InfraestructuraComputacional/Seguimiento/7/2%20(2).jpg" style="max-width:100%;">

3. Luego se usa enable para la persistencia con systemctl enable mariadb

<img src= "https://github.com/dannamayac/AdministracionSOLINUX-G1N/blob/main/InfraestructuraComputacional/Seguimiento/7/3.jpg" style="max-width:100%;">

4. Verificamos el estatus mediante systemctl status mariadb

<img src= "https://github.com/dannamayac/AdministracionSOLINUX-G1N/blob/main/InfraestructuraComputacional/Seguimiento/7/5.png" style="max-width:100%;">

5. Se configura la máquina virtual para conexiones remotas

<img src= "https://github.com/dannamayac/AdministracionSOLINUX-G1N/blob/main/InfraestructuraComputacional/Seguimiento/7/5.png" style="max-width:100%;">

6. Se verifica que funcione el despliegue

<img src= "https://github.com/dannamayac/AdministracionSOLINUX-G1N/blob/main/InfraestructuraComputacional/Seguimiento/7/6.jpg" style="max-width:100%;">

