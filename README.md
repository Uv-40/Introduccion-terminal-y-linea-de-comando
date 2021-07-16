# Introduccion-terminal-y-linea-de-comando

- [Modulo 1 primeros pasos](#Modulo-1-primeros-pasos)
  - [Clase 1 Que es la terminal?](#clase-1-que-es-la-terminal-?)
  - [Clase 2 Aprendiendo a caminar la terminal](#clase-2-aprendiendo-a-caminar-la-terminal)






## Modulo 1: primeros pasos 

### Clase 1 Que es la terminal?

### Pero qué es...

Es una interfaz gráfica que simula una linea de comandos y cuando hablamos de una línea de comandos nos referimos a una `shell`.

- **Terminal**: es la ventanita que nos muestra el prompt. Este aloja la shell.
- **Linea de comandos**: programa que toma comandos y los pasa al sistema operativo para hacer algo.

Las razones para aprender a usarla son:

1. Tenemos mucha **flexibilidad** ya que podemos hacer procesos dentro de nuestra computadora de una forma más eficiente, mover grandes volúmenes de datos de forma rápida, así como hacer copias e incluso programar procesos que se ejecuten en cierto tiempo
2. Normalmente hacer cosas en la terminal como copiar archivos o buscarlos tiende a ser mucho más rápido que hacerlo a través de una interfaz gráfica. Por lo tanto podemos decir que tenemos una **velocidad** mayor al realizar dichos procesos en la terminal.
3. **No siempre contaremos con una interfaz gráfica** o puede llegar a fallar.

### Tipos de lineas de comandos

- Bourne Shell
- Bash Shell
- Z Shell
- C Shell
- Korn Shell
- Fish Shell
- PowerShell

Las más populares


### Clase 2: Aprendiendo a caminar la terminal

El sistema de archivos, será el árbol por el que nos estaremos moviendo en la terminal.

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ff586baf-743a-4887-a1d4-76628b9ba17d/2._Slides.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ff586baf-743a-4887-a1d4-76628b9ba17d/2._Slides.png)

Aquí se encuentran los archivos del sistema operativo, así como también los ejecutables, controladores, archivos de configuración, etcétera.

En la carpeta `home` es donde se encuentran los usuarios del sistema operativo. Dentro de la terminal identificamos esta carpeta con el símbolo llamado virgulilla `~`.

#### Primeros comandos

| **Comando** | Accion |
| ----------- | ------ |
| ls :  | Lista los archivos y carpetas del directorio. |
| ls -l : | Lista los archivos y carpetas con la información adicional. |
| ls -lh :|Lista los archivos y carpetas con la información legible para humanos. |
| cd : | Mueve la terminal al directorio `home` del usuario. |
| cd {folder} : | Mueve la terminal al directorio indicado. |
| clear : | Limpia la pantalla de la terminal (shortcut: `Control + L`). |
| pwd : | (print working diretory) Imprime la ruta actual en la que nos encontramos en la terminal. |
| file {name_file} : | Describe el tipo de archivo que le pasamos como parámetro. |

#### Rutas relativas

Tenemos dos parámetros que nos ayudan a trabajar con las rutas en la terminar, estos parámetros son de rutas relativas. Los conocemos como `.` y `..`.

El primer de ellos nos ubica en el directorio actual y el segundo nos regresa un directorio.



### Clase 3: Manipulando archivos y directorios

### Listando elementos

Comando

ls -la

ls -lS

ls -lr

tree

tree -L {#}

Acción

Lista todos los elementos del directorio, incluidos los ocultos.

Lista todos los elementos iniciando por los más pesados.

Lista todos los elementos de forma inversa.

Despliega todos nuestros directorios como un árbol.

Despliega los elementos que se encuentren en el nivel indicado.

### Manipulación de elementos

**Comando**

mkdir {folder}

touch {file}

cp {original} {copia}

mv {file} {path}

mv {name} {new_name}

rm {file}

rm -i {file}

rm -r {folder}

**Acción**

Crea un nuevo directorio con el nombre indicado.

Crea un nuevo archivo con el nombre indicado.

Copia un archivo.

Mueve el archivo a la ubicación deseada.

Renombra el archivo o directorio.

Elimina el archivo indicado.

Pide confirmación antes de eliminar el archivo.

Elimina el directorio indicado.
