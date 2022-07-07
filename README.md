# CONSOLA LINUX

CTRL+ALT+T = Abrir terminal

## Comandos

| comando                   | descripcion                                    |
| ------------------------- | ---------------------------------------------- |
| `(sh)`                    | son los ejecutables de Linux                   |
| `sudo +comando`           | aplica en modo admin                           |
| `clear`                   | limpia la consola                              |
| `kill -9 numerodeproceso` | mata al proceso (se ven con ps –ef)            |
| `exit`                    | sale de la terminal                            |
| `shutdown –h`             | Linux se apaga en un minuto                    |
| `shutdown –h 0`           | Linux se apaga inmediatamente (o shutdown now) |

## PARA ARCHIVOS

| comando                          | descripcion                                                                                                                                                           |
| -------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `mkdir`                          | crea un directorio                                                                                                                                                    |
| `sudo +comando`                  | aplica en modo admin                                                                                                                                                  |
| `slear`                          | limpia la consola                                                                                                                                                     |
| `touch nombrearchivo`            | crea un archivo vacío                                                                                                                                                 |
| `touch archivo.txt`              | permite crear un archivo, con la extensión mencionada                                                                                                                 |
| `> archivo.txt `                 | igual que touch, crea un archivo                                                                                                                                      |
| `< archivo.txt`                  | crea un archivo, o vacía (reemplaza) uno existente con ese nombre.                                                                                                    |
| `echo "texto" > archivo.txt`     | si existe archivo.txt, le escribe el texto, sino, crea un archivo nuevo con el texto de las comillas. Si hacemos esto en un archivo creado, sobrescribe el contenido. |
| `echo "texto" >> archivo.txt`    | Escribe el texto en otra línea, en el archivo.                                                                                                                        |
| `cat archivo.txt`                | nos muestra el contenido del archivo                                                                                                                                  |
| `cat archivo.txt more`           | nos muestra el contenido del archivo pero más detallado                                                                                                               |
| `less archivo`                   | igual que more pero podemos mover con flechitas                                                                                                                       |
| `head archivo`                   | nos muestra las primeras 10 lineas del archivo.                                                                                                                       |
| `tail archivo`                   | nos muestra las ultimas 10 lineas de un archivo de texto.                                                                                                             |
| `./archivo.txt`                  | con ./ le decimos a Linux que ejecute el directorio a partir de donde estamos parados en este momento. Ejecuta el archivo, debemos estar en la carpeta del archivo.   |
| `sh archivo`                     | ejecuta el archivo, igual que ./                                                                                                                                      |
| `cp archivo.txt /carpeta1`       | copia el archivo en la carpeta indicada                                                                                                                               |
| `cp –r /carpeta1 /carpeta2`      | copia el directorio en la carpeta indicada (-r es para directorios)                                                                                                   |
| `mv archivo.txt /carpeta1`       | mueve el archivo a la carpeta deseada                                                                                                                                 |
| `mv directorio2 dir2`            | le cambia el nombre al directorio                                                                                                                                     |
| `rm archivo.txt`                 | remueve el archivo                                                                                                                                                    |
| `rm –r carpeta`                  | borra la carpeta                                                                                                                                                      |
| `rm –rf directorio`              | remueve el directorio y su contenido (la f es de forzar, borra aunque tenga contenido)                                                                                |
| `chmod 777 archivo o directorio` | le da permisos de lectura, escritura y ejecución a todos.                                                                                                             |

## Propietario-Grupo-Otros

- Read – 4

- Write – 2

- Execute – 1

## Crear carpeta y copiar un archivo

**mkdir carpeta**

**touch archivo.html**

**cp archivo.html ./carpeta/** (si la carpeta está dentro del mismo nivel que el archivo)

**cp archivo.html ../carpeta** (Si la carpeta está un nivel abajo que el archivo)

**ls carpeta**

## Para copiar o mover

**cp Músicaa ../basura**

**cp /home/manjaro/Escritorio/poronga/archivo.txt /home/manjaro/Música/**

## PARA MOVERSE

| comando               | descripcion                                                                           |
| --------------------- | ------------------------------------------------------------------------------------- |
| `cd /carpeta/carpeta` | nos lleva a la carpeta deseada                                                        |
| `cd directorio`       | nos lleva al directorio/carpeta que queremos ir (hay que mirar donde estamos parados) |
| `cd`                  | nos vuelve al directorio home de nuestra cuenta                                       |
| `cd ~`                | nos devuelve al home de nuestra cuenta.                                               |
| `cd ..`               | nos sube un directorio más a donde estamos                                            |
| `cd ../`              | baja un escalón                                                                       |

## INFORMATIVOS

| comando                      | descripcion                                                                                                                                                   |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `pwd`                        | nos va a decir en que directorio nos encontramos                                                                                                              |
| `ls -l`                      | nos va a dar un listado de los archivos y directorios que tengamos en donde estemos parados.                                                                  |
| `ls –alh`                    | la a muestra todos los archivos en ese directorio incluyendo los ocultos (empiezan con .), la l los muestra en lista, y la h muestra el peso de los archivos. |
| `ls la`                      | nos da información de los archivos q tengamos en donde estamos parado                                                                                         |
| `du –sh`                     | muestra cuanto espacio estamos ocupando en el directorio.                                                                                                     |
| `whoami`                     | nos va a decir con que cuenta estamos logueados                                                                                                               |
| `ps`                         | listado de procesos que están ejecutándose en la pc                                                                                                           |
| `ps –ef`                     | listado con todos los procesos                                                                                                                                |
| `ps –ef grep Chrome`         | busca, por ejemplo, todos los procesos Chrome abiertos                                                                                                        |
| `top`                        | sirve para monitorear el equipo, vemos los procesos, memoria, etc (salimos con la tecla Q)                                                                    |
| `man cp`                     | lnos muestra la información de los comandos, copy, o cual sea                                                                                                 |
| `ip -4 a`                    | muestra todas las interfaces de red, versión ip4                                                                                                              |
| `ip a`                       | muestra todas, también las ip6c                                                                                                                               |
| `echo $PATH`                 | te muestra la ruta de instalación.                                                                                                                            |
| `env`                        | nos da información del sistema                                                                                                                                |
| `export PATH=$PATH:/otp/bin` | le agrega a la ruta de PATH, el /otp                                                                                                                          |
| `who`                        | nos indica las cuentas activas en este equipo en este momento.                                                                                                |
| `w`                          | igual que who pero con mas info.                                                                                                                              |

**BUSCADORES**

| comando                         | descripcion                                                                      |
| ------------------------------- | -------------------------------------------------------------------------------- |
| `find`                          | nos permite encontrar archivos.                                                  |
| `find .`                        | significa que la búsqueda es en el directorio actual                             |
| `find . –name "asd"`            | busca el archivo en el directorio actual, e indica la ruta.                      |
| `find . –iname "aSd"`           | busca el archivo en el directorio actual, sin importar las mayúsculas o minus.   |
| `find . –name "archivo.tx?"`    | el ? sirve como un comodín, encuentra los archivos completando el dato faltante. |
| `find . –name *.txt`            | encuentra todos los archivos .txt sin importar el nombre                         |
| `find /`                        | indica que la búsqueda es en todo el sistema.                                    |
| `find / -name *.txt`            | busca en todo el sistema todos los .txt                                          |
| `find ./Escritorio –type d`     | busca solo los tipo d (directorios) en la carpeta indicada.                      |
| `find . –size -10M –name *.txt` | busca todos los txt menor tamaño a 10mb                                          |

## GREP (buscar en la carpeta donde se encuentra el archivo)

| comando                   | descripcion                                                     |
| ------------------------- | --------------------------------------------------------------- |
| `grep –i asd archivo.txt` | busca "asd" en el archivo indicado, debemos estar en la carpeta |
| `grep –l asd ./* `        | busca “asd” en todos los archivos de la carpeta donde estemos   |
| `grep asd *`              | busca “asd” en los archivos de la carpeta donde estemos         |
| `grep –s asd *`           | busca “asd” en los archivos, evitando los que no tiene permisos |

## Para buscar algún error dentro del sistema:

| comando                | descripcion                                                                                                  |
| ---------------------- | ------------------------------------------------------------------------------------------------------------ |
| `grep error *.log`     | busca "error" en todos los ficheros .log                                                                     |
| `grep –s error *.log ` | busca "error" en los archivos, evitando los que no tiene permisos                                            |
| `grep –sl error *.log` | busca "error" en los ficheros donde se produzca esta coincidencia                                            |
| `grep –sc error *.log` | busca "error" en los ficheros donde se produzca esta coincidencia e indica cuantas veces aparece en cada uno |
| `grep –si error *.log` | busca "error" en los ficheros donde se produzca esta coincidencia, sin importar mayus o minúsculas.          |

## Escrbir código en Markdown

```js
const ian = "pt";
```
