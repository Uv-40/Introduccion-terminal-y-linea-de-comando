# Introduccion-terminal-y-linea-de-comando

- [Modulo 1 primeros pasos](#Modulo-1-primeros-pasos)
  - [Clase 1 Que es la terminal?](#clase-1-que-es-la-terminal-?)
  - [Clase 2 Aprendiendo a caminar la terminal](#clase-2-aprendiendo-a-caminar-la-terminal)
  - [Clase 3: Manipulando archivos y directorios](#Clase-3-Manipulando-archivos-y-directorios)
  - [Clase 4: Explorando el contenido de nuestros archivos](#Clase-4-Explorando-el-contenido-de-nuestros-archivos)
  - [Clase 5: Que es un comando?](Clase-5-Que-es-un-comando?)
  - [Clase 6: Wildcards](clase-6-wildcards)






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

#### Listando elementos

| Comando | Accion |
| ------- | ------ |
| ls -la : | Lista todos los elementos del directorio, incluidos los ocultos. |
| ls -lS : | Lista todos los elementos iniciando por los más pesados. |
| ls -lr : | Lista todos los elementos de forma inversa. |
| tree : | Despliega todos nuestros directorios como un árbol. |
| tree -L {#} | Despliega los elementos que se encuentren en el nivel indicado. |


#### Manipulación de elementos

| **Comando** | Accion |
| ----------- | ------ |
| mkdir {nombre folder} | Crea una carpeta |
| touch {Nombre file} | Crea un archivo |
| cp {original} | hace una copia de arcchivos {copia} |
| mv {file} {path} | Mueve el archivo al path que se escribe |
| mv {name} {new_name} | este comando permite cambiar el nombre del archivo |
| rm {file} | elimina el archivo |
| rm -i {file} | Pide confirmación antes de eliminar el archivo. |
| rm -r {folder} | Elimina el directorio indicado. |



### Clase 4: Explorando el contenido de nuestros archivos

La terminal nos permite explorar archivos desde ella misma, así evitamos abrirlos por completo. Los comandos para explorar archivos están listados a continuación.

### Comandos de la clase

| **Comando** | Accion |
| ----------- | ------ |
| head {file} | Muestra las primeras lineas del archivo |
| head {file} -n {#} | Muetra la primeras lineas del archivo segun el numero que se ponga luego de la n |
| tail {file} | Muestra as ultimas lineas del archivo |
| tail {file} -n {#} | Muestra las ultimas lineas segun el numero que se ponga luego de la n |
| less {file} | Muestra todo el archivo de texto seleccionado. |
| open | Abre un archivo desde la terminal (MacOs). |
| xdg-open | Abre un archivo desde la terminal (Linux). |
| nautilus | Abrir el sistema de archivos (Linux). |

Para detener un proceso que se esté ejecutando en la terminal basta con utilizar la combinación de teclas `ctrl + c` para interrumpirlo.


### Clase 5: Que es un comando?

Un comando puede ser:
  - Un programa ejecutable
  - Un comando de utilidad shell
  - Una funcion shell
  - un alias

### Clase 6: Wildcards

Son una serie de caracteres especiales que nos permiten encontrar patrones o hacer busquedas mas avanzadas.

Ej: todos los archivos de python o excel 

comando ls *.{tipo de archivo} 
ej: ls*.txt (nos muestra todos los archivos de formato txt

comando ls datos*
muestra todos los archivos que contengan la palabra datos

comando ls datos?
muestra los archivos que tengan el nombre datos + un caracter (el ? indica el numero de caracteres adiconales)


## Modulo 2: Empezando a correr


### Clase 7: Redirecciones: como funciona la shell

Las redirecciones son comandos que nos permiten manejar la entradas y salidas de la terminal 

stdin  (0) = standard input  = provee comandos de entrada, y se describen en linux con el codigo 0.
stdout (1) = standard output = muestra comandos de salida, descritos en linux con el codigo 1.
stderr (2) = standard error  = provee salidas de errores de los comandos, descritos en linux con el codigo  2.

| Simbolo | Descripcion |
| ------- | ----------- |
| > | Redirecciona el stdout hacia un *archivo*. Lo crea si no existe, si existe lo sobreescribe. |
| >> | Redirecciona stdout hacia un *archivo*. Lo crea si no existe, si existe concatena la salida al final de este. |
| < | redirecciona stdin desde un archivo. El contenido de un archivo es la entrada o input del comando. |
| 2> o 2>> | Redirecciona stderr hacia un archivo. Crea (>) o concatena (>>) la salida de errores a un archivo. |
| 1>&2 | redirecciona stdout hacia donde stderr apunte. |

### Clase 8: Redirecciones pipe operator

El pipe operator nos permite hacer que el stdout pase como stdinp a otro comando, lo cual nos permite generar filtros, encadenamisntos o funcionalidades que pueden terminar por un archivo.

Comando ECHO = genera un standard output en la terminal de cualquier cosa que le escribamos.
Comando CAT <archivo 1> <archivo 2> = permite concatenar la informacion de 2 archivos que pongamos.

El pipe operator nos permite que el stdout de un comando se convierta en el stdin de otro comando


### Clase 9: Encadenando comandos: operadores de control

Son simbolos reservados por la terminal que nos permiten ejecutar mas de un comando o encadenarlos

Ej: crear un carpeta y movernos a ella
    ver si se cumple un comando para que se ejecute otro
    
| Comando | Funcion |
| ------- | ------- |
| comandos separados por ; | Con el punto y coma se pueden separar diferentes comandos para que se ejecuten de manera sincrona es decir uno detras de otro. |
| comandos separados por & | Con este comando se pueden separar diferentes funciones para que se ejecuten de manera asincrona es decir todos al tiempo cada una genere un hilo distinto |
| comandos separados por && | comando (AND) ejecuta cada comando solo si el anterior ya se ejecuto exitosamente |
| comandos separados por // | Comando (OR) ejecuta cada comando hasta que uno sea exitoso y descarta los comandos que se encuentren después del que se ejecuto exitosamente |
    

### Clase 10: Como se manejan los permisos

| Atributo | Tipo de archivo |
| -------- | --------------- |
| - | Un archivo normal |
| d | Un directorio |
| l | link simbolico |
| b | archivo de bloque especial. son archivos que manejan la informacion de los bloques de datos como una USB |

![Permisos en linux](https://user-images.githubusercontent.com/25805919/126578837-2adf78dc-376e-48c3-a4bb-d5371c003c1a.PNG)
