# CONSOLA LINUX

CTRL+ALT+T = Abrir terminal

## Comandos

| comando                   | descripcion                                    |
| ------------------------- | ---------------------------------------------- |
| `(sh)`                    | son los ejecutables de Linux                   |
| `Sudo +comando`           | aplica en modo admin                           |
| `Clear`                   | limpia la consola                              |
| `Kill -9 numerodeproceso` | mata al proceso (se ven con ps –ef)            |
| `Exit`                    | sale de la terminal                            |
| `Shutdown –h`             | Linux se apaga en un minuto                    |
| `Shutdown –h 0`           | Linux se apaga inmediatamente (o shutdown now) |

## PARA ARCHIVOS

| comando                                               | descripcion                                                                                                                                                           |
| ----------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `mkdir`                                               | crea un directorio                                                                                                                                                    |
| `Sudo +comando`                                       | aplica en modo admin                                                                                                                                                  |
| `Clear`                                               | limpia la consola                                                                                                                                                     |
| `Touch nombrearchivo`                                 | crea un archivo vacío                                                                                                                                                 |
| `Touch archivo.txt`                                   | permite crear un archivo, con la extensión mencionada                                                                                                                 |
| `> archivo.txt `                                      | igual que touch, crea un archivo                                                                                                                                      |
| `&lt; archivo.txt`                                    | crea un archivo, o vacía (reemplaza) uno existente con ese nombre.                                                                                                    |
| `Echo &quot;algún texto&quot; \&gt; archivo.txt`      | si existe archivo.txt, le escribe el texto, sino, crea un archivo nuevo con el texto de las comillas. Si hacemos esto en un archivo creado, sobrescribe el contenido. |
| `Echo &quot;algún texto&quot; \&gt;\&gt; archivo.txt` | Escribe el texto en otra línea, en el archivo.                                                                                                                        |
| `Cat archivo.txt`                                     | nos muestra el contenido del archivo                                                                                                                                  |
| `Cat archivo.txt more`                                | nos muestra el contenido del archivo pero más detallado                                                                                                               |
| `Less archivo`                                        | igual que more pero podemos mover con flechitas                                                                                                                       |
| `Head archivo`                                        | nos muestra las primeras 10 lineas del archivo.                                                                                                                       |
| `Tail archivo`                                        | nos muestra las ultimas 10 lineas de un archivo de texto.                                                                                                             |
| `./archivo.txt`                                       | con ./ le decimos a Linux que ejecute el directorio a partir de donde estamos parados en este momento. Ejecuta el archivo, debemos estar en la carpeta del archivo.   |
| `Sh archivo`                                          | ejecuta el archivo, igual que ./                                                                                                                                      |
| `Cp archivo.txt /carpeta1`                            | copia el archivo en la carpeta indicada                                                                                                                               |
| `Cp –r /carpeta1 /carpeta2`                           | copia el directorio en la carpeta indicada (-r es para directorios)                                                                                                   |
| `Mv archivo.txt /carpeta1`                            | mueve el archivo a la carpeta deseada                                                                                                                                 |
| `Mv directorio2 dir2`                                 | le cambia el nombre al directorio                                                                                                                                     |
| `Rm archivo.txt`                                      | remueve el archivo                                                                                                                                                    |
| `Rm –r carpeta`                                       | borra la carpeta                                                                                                                                                      |
| `Rm –rf directorio`                                   | remueve el directorio y su contenido (la f es de forzar, borra aunque tenga contenido)                                                                                |
| `Chmod 777 archivo o directorio`                      | le da permisos de lectura, escritura y ejecución a todos.                                                                                                             |

## Propietario-Grupo-Otros

- Read – 4

- Write – 2

- Execute – 1

## CREAR CARPETA Y COPIAR UN ARCHIVO

**Mkdir carpeta**

**Touch archivo.html**

**Cp archivo.html ./carpeta/** (si la carpeta está dentro del mismo nivel que el archivo)

**Cp archivo.html ../carpeta** (Si la carpeta está un nivel abajo que el archivo)

**Ls carpeta**

## PARA COPIAR PIOLA o mover

**Cp Músicaa ../basura**

**cp /home/manjaro/Escritorio/poronga/archivo.txt /home/manjaro/Música/**

## PARA MOVERSE

| comando               | descripcion                                                                           |
| --------------------- | ------------------------------------------------------------------------------------- |
| `Cd /carpeta/carpeta` | nos lleva a la carpeta deseada                                                        |
| `Cd directorio`       | nos lleva al directorio/carpeta que queremos ir (hay que mirar donde estamos parados) |
| `Cd`                  | nos vuelve al directorio home de nuestra cuenta                                       |
| `Cd ~`                | nos devuelve al home de nuestra cuenta.                                               |
| `Cd ..`               | nos sube un directorio más a donde estamos                                            |
| `Cd ../`              | baja un escalón                                                                       |

## INFORMATIVOS

| comando                      | descripcion                                                                                                                                                   |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `Pwd`                        | nos va a decir en que directorio nos encontramos                                                                                                              |
| `Ls -L`                      | nos va a dar un listado de los archivos y directorios que tengamos en donde estemos parados.                                                                  |
| `Ls –alh`                    | la a muestra todos los archivos en ese directorio incluyendo los ocultos (empiezan con .), la l los muestra en lista, y la h muestra el peso de los archivos. |
| `Ls la`                      | nos da información de los archivos q tengamos en donde estamos parado                                                                                         |
| `Du –sh`                     | muestra cuanto espacio estamos ocupando en el directorio.                                                                                                     |
| `Whoami`                     | nos va a decir con que cuenta estamos logueados                                                                                                               |
| `Ps`                         | listado de procesos que están ejecutándose en la pc                                                                                                           |
| `Ps –ef`                     | listado con todos los procesos                                                                                                                                |
| `Ps –ef grep Chrome`         | busca, por ejemplo, todos los procesos Chrome abiertos                                                                                                        |
| `Top`                        | sirve para monitorear el equipo, vemos los procesos, memoria, etc (salimos con la tecla Q)                                                                    |
| `Man cp`                     | lnos muestra la información de los comandos, copy, o cual sea                                                                                                 |
| `Ip -4 a`                    | muestra todas las interfaces de red, versión ip4                                                                                                              |
| `Ip a`                       | muestra todas, también las ip6c                                                                                                                               |
| `Echo $PATH`                 | te muestra la ruta de instalación.                                                                                                                            |
| `Env`                        | nos da información del sistema                                                                                                                                |
| `Export PATH=$PATH:/otp/bin` | le agrega a la ruta de PATH, el /otp                                                                                                                          |
| `Who`                        | nos indica las cuentas activas en este equipo en este momento.                                                                                                |
| `W`                          | igual que who pero con mas info.                                                                                                                              |

**BUSCADORES**

Find = nos permite encontrar archivos.

Find . = significa que la búsqueda es en el directorio actual

Find . –name &quot;asd&quot; = busca el archivo en el directorio actual, e indica la ruta.

Find . –iname &quot;aSd&quot; = busca el archivo en el directorio actual, sin importar las mayúsculas o minus.

Find . –name &quot;archivo.tx?&quot; = el ? sirve como un comodín, encuentra los archivos completando el dato faltante.

Find . –name \*.txt = encuentra todos los archivos .txt sin importar el nombre

Find / = indica que la búsqueda es en todo el sistema.

Find / -name \*.txt = busca en todo el sistema todos los .txt

Find ./Escritorio –type d = busca solo los tipo d (directorios) en la carpeta indicada.

Find . –size -10M –name \*.txt = busca todos los txt menor tamaño a 10mb

GREP (buscar en la carpeta donde se encuentra el archivo)

Grep –i asd archivo.txt = busca &quot;asd&quot; en el archivo indicado, debemos estar en la carpeta

Grep –l asd ./\* = busca &quot;asd&quot; en todos los archivos de la carpeta donde estemos

Grep asd \* = busca &quot;asd&quot; en los archivos de la carpeta donde estemos

Grep –s asd \* = busca &quot;asd&quot; en los archivos, evitando los que no tiene permisos

Para buscar algún error dentro del sistema:

Cd

Cd /var/log

Grep error \*.log = busca &quot;error&quot; en todos los ficheros .log

Grep –s error \*.log = busca &quot;error&quot; en los archivos, evitando los que no tiene permisos

Grep –sl error \*.log = busca &quot;error&quot; en los ficheros donde se produzca esta coincidencia`

Grep –sc error \*.log = busca &quot;error&quot; en los ficheros donde se produzca esta coincidencia e indica cuantas veces aparece en cada uno.

Grep –si error \*.log = busca &quot;error&quot; en los ficheros donde se produzca esta coincidencia, sin importar mayus o minúsculas.

```js
const ian = 'pt'
```
