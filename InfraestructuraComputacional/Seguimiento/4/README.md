Creación del archivo README.md
1.	 Crear dos grupos llamados: profesor y estudiante
Para iniciar con la actividad debemos acceder al super usuario con el comando sudo -s, posteriormente, escribimos la contraseña.
A continuación usamos el comando groupadd -r profesor && groupadd -r estudiante, para continuar, usamos pwd para conocer la ruta donde nos encontramos y luego retrocedemos dos veces atrás con cd.

<img src= "InfraestructuraComputacional\Seguimiento\4\t41.png" style="max-width:100%;">

2. Crear tres usuarios llamados: diana, claudia y laura.

<img src= "InfraestructuraComputacional\Seguimiento\4\t42.png" style="max-width:100%;">

El paso a continuación, es crear 3 usuarios usando el comando usaradd diana && user add claudia && useradd Laura. Después de lo realizado anteriormente, listamos y confirmamos si fueron creados por el comando cat etc /passwd y verificamos si se encuentran en el listado.

<img src= "InfraestructuraComputacional\Seguimiento\4\t43.png" style="max-width:100%;">

3. Conociendo que: diana es un profesor; laura es una estudiante yclaudia es un profesor y un estudiante. Adicione todos los usuarios a los grupos correspondientes.

Añadimos a los usuarios creados anteriormente,  los grupos que corresponden usando los siguientes comandos usermod -g profesor diana usermod -g estudiante laura como claudia es un profesor y un estudiante usamos el siguiente comando con las banderas -a y -G usermod -a -G estudiante claudia usermod -a -G profesor Claudia, luego usamos el comando groups para verificar que los usuarios se encuentren añadidos correctamente.

<img src= "InfraestructuraComputacional\Seguimiento\4\T44.png" style="max-width:100%;">

4. Cree dos directorios, uno para profesores (solo los profesores tienen acceso) y otro para estudiantes (profesores y estudiantes tienen acceso). Asegúrese de asignar los permisos.

Volvemos a la ruta cd home/ y creamos los directorios usando los comandos mkdir profesores y mkdis estudiantes. 

<img src= "InfraestructuraComputacional\Seguimiento\4\T45.png" style="max-width:100%;">

con el comando 'ls -l' con el objetivo de listar los directorios y evidenciar sus permisos observamos que el root tiene los permisos que requiere estos directorios.

<img src= "InfraestructuraComputacional\Seguimiento\4\T46.png" style="max-width:100%;">

Una vez creado los directorios debemos generar el permiso a los mismos para que los grupos estudiante y profesor puedan ser modificados en cada directorio correspondiente, para lo anterior, se lleva a cabo de dos formas diferentes, una se realiza con el comando 'chgrp + nombre del grupo + el nombre del directorio'.
La otra forma de realizarlo es por medio de 'chown + nombre del grupo + nombre del directorio'. Para el desarrollo de este ejercicio elegiremos esta forma.
Por último, escribimos el comando 'ls -l' y verificamos que los grupos estudiante y profesor también tengan los permisos que le pertenecen a estos directorios.

<img src= "InfraestructuraComputacional\Seguimiento\4\T47.png" style="max-width:100%;">
<img src= "InfraestructuraComputacional\Seguimiento\4\T48.png" style="max-width:100%;">

5. Verifique los permisos anteriores, usando las cuentas de los usuarios ya creados

Para verificar los permisos debemos loguearnos con diferentes usuarios y tratando de ingresar a los directorios. En la siguiente imagen se aprecia que Claudia y Diana tienen ingreso al directorio profesores por que pertenecen al grupo profesor, pero laura no porque pertenece al grupo estudiante.

<img src= "InfraestructuraComputacional\Seguimiento\4\T49.png" style="max-width:100%;">
<img src= "InfraestructuraComputacional\Seguimiento\4\T50.png" style="max-width:100%;">
<img src= "InfraestructuraComputacional\Seguimiento\4\T51.png" style="max-width:100%;">

6. Use un editor de texto para crear archivos en los respectivos directorios, usando diferentes usuarios.

<img src= "InfraestructuraComputacional\Seguimiento\4\T52.png" style="max-width:100%;">
<img src= "InfraestructuraComputacional\Seguimiento\4\T53.png" style="max-width:100%;">
<img src= "InfraestructuraComputacional\Seguimiento\4\T54.png" style="max-width:100%;">

7. Como super usuario, cambie de dueño los archivos creados

Usamos el comando chown+nombre usuario+ nombre del archivo del usuario a cambiar /h2>
listamos con el comando ls -l para verificar los permisos
Cambiamos los permisos de claudia a diana y luego de claudia a diana como se puede ver en la imagen.

<img src= "InfraestructuraComputacional\Seguimiento\4\T55.png" style="max-width:100%;">

8. Usando diferentes terminales, entre al sistema con los diferentes usuarios:

<img src= "InfraestructuraComputacional\Seguimiento\4\T56.png" style="max-width:100%;">

9. Usando diferentes terminales, entre al sistema con los diferentes usuarios.

El objetivo para este ejercicio es que se ingrese mal las claves en el nombre del usuario.

<img src= "InfraestructuraComputacional\Seguimiento\4\T57.png" style="max-width:100%;">

10. Determine la cantidad de veces que el estudiante laura ingreso al sistema.

<img src= "InfraestructuraComputacional\Seguimiento\4\T58.png" style="max-width:100%;">

11. Comprima el contenido del directorio de los profesores en profesore.tgz y el contenido del directorio de los estudiante en un archivo estudiantes.zip.

<img src= "InfraestructuraComputacional\Seguimiento\4\T59.png" style="max-width:100%;">

12. Cree un alias para cambiar la clave del usuario diana.

<img src= "InfraestructuraComputacional\Seguimiento\4\T60.png" style="max-width:100%;">