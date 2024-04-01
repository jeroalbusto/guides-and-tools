# GNU/Linux :penguin: :computer:

Linux es un sistema operativo open source gratuito que se lanza en virtud de la Licencia Pública General de GNU (GPL). Cualquier persona puede ejecutar, estudiar, modificar o redistribuir el código fuente, e incluso comercializar las copias de su código modificado, siempre y cuando lo haga con la misma licencia.

## Terminal
En linux la terminal es uno de los programas mas utilizados e importantes es una interfaz de línea de comandos que permite a los usuarios interactuar con el sistema operativo mediante comandos de texto. Algunas de las variantes más populares de terminales en Linux incluyen:

- Bash (Bourne Again Shell): Es el intérprete de comandos predeterminado en la mayoría de las distribuciones de Linux, con soporte para scripting.

- Zsh (Z Shell): Es una shell de Unix interactiva y un potente intérprete de comandos similar a Bash, pero con características adicionales y una sintaxis más avanzada. Zsh es altamente personalizable y es popular entre los usuarios avanzados por su amplia gama de complementos y características.

Se instala usando el comando:
```bash
sudo apt-get install zsh
```
Configuración de Zsh como Shell Predeterminada:
```bash
chsh -s $(which zsh)
```

- Fish (Friendly Interactive Shell): Es una shell de línea de comandos diseñada para ser fácil de usar y amigable para los principiantes. Tiene una sintaxis más sencilla y predictiva que Bash y Zsh, y ofrece características como la finalización automática de comandos y la visualización de sugerencias mientras escribes.

Se instala usando el comando:
```bash
sudo apt-get install fish
```
Configuración de Fish como Shell Predeterminada:
```bash
chsh -s $(which fish)
```

---

### Curl

Curl es una herramienta de línea de comandos y una biblioteca de transferencia de datos utilizada para transferir datos a través de varios protocolos. Puede manejar protocolos como HTTP, HTTPS, FTP, FTPS, SCP, SFTP, TFTP, LDAP, DICT, TELNET, FILE, IMAP, SMTP, POP3, RTSP y otros. Se usa para descargar archivos desde internet.

Para instalar curl se usa:
```bash
sudo apt-get install curl
```
Para verificar si curl se ha instalado correctamente, se usa:
```bash
curl --version
```
Esto mostrará la versión de curl instalada en tu sistema, lo que confirma que la instalación ha sido exitosa.

---

### Instalar archivos .deb

 Una vez que hayas descargado el archivo .deb, puedes instalarlo usando el comando APT. Abre una terminal y navega hasta la ubicación donde descargaste el archivo .deb, luego ejecuta el siguiente comando:
 ```bash
 sudo apt-get install ./nombre_archivo.deb
 ```
 Para desinstalar un paquete .deb con APT:
 ```bash
 sudo apt-get remove nombre_archivo
 ```

---

### Comandos Basicos de la Terminal

Para limpiar la pantalla de la terminal, eliminando cualquier texto o salida que esté presente
```bash
clear
```
Otra alternativa es el comando Ctrl + L (tecla Control más la letra "L") es un atajo de teclado que también se utiliza para limpiar la pantalla de la terminal, similar al comando clear. En la mayoría de las terminales, al presionar Ctrl + L, se borra el contenido de la pantalla y se desplaza hacia arriba, dejando una ventana de visualización limpia.

Mostrar la ruta del directorio actual
```bash
pwd
```
Moverse o cambiar de directorio
```bash
cd nombre_directorio
```
Volver un directorio o dos
```bash
cd ..

cd ...
```
Listar los archivos y directorios en el directorio actual
```bash
ls
```
Listar los archivos y directorios en el directorio actual con sus permisos, autor, fecha, hora, etc
```bash
ls -l
```
Listar los archivos y directorios en el directorio actual, y los ocultos
```bash
ls -a
```
Crear un directorio
```bash
mkdir nombre_directorio
```
Crear un archivo vacio
```bash
touch nombre_archivo
```
Actualizar la fecha de modificacion de un archivo existente
```bash
touch -t año-mes-día-hora-minuto nombre_archivo
```
Mostrar el contenido de un archivo
```bash
cat nombre_archivo
```
Copiar archivos o directorios
```bash
cp nombre destino
```
Mover archivos o directorios
```bash
mv nombre destino
```
Eliminar archivos
```bash
rm nombre_archivo
```
Eliminar directorio vacio
```bash
rmdir nombre_directorio
```
Eliminar directorio y su contenido
```bash
rm -r nombre_directorio
```
Cambiar los permisos de un archivo o directorio
```bash
chmod permisos nombre_archivo
```
Puedes especificar los permisos simbólicamente utilizando las letras u (propietario), g (grupo) y o (otros), junto con los operadores + (añadir permisos), - (eliminar permisos) y = (establecer permisos).

- Lectura (r)
- Escritura (w)
- Ejecución (x)

Por ejemplo, para dar permisos de escritura al grupo y otros, puedes usar:
```bash
chmod go+w archivo
```
Crear o extraer archivos comprimidos
```bash
tar -cvf archivo.tar directorio (crear un archivo)

tar -xvf archivo.tar (extraer un archivo)
```
Listar el contenido de un archivo tar
```bash
tar -tvf archivo.tar
```

Mostrar el espacio en disco disponible 
```bash
df
```
Mostrar información en un formato más legible para humanos, mostrando los tamaños en unidades más fáciles de entender (por ejemplo, KB, MB, GB)
```bash
df -h
```

Mostrar el uso del disco de archivos y directorios
```bash
du
```
Mostrar la ruta del archivo ejecutable de un programa
```bash
which nombre_programa
``` 
Terminar un proceso
```bash
kill PID_proceso
```
kill enviara una señal al proceso identificado por su PID (Identificador de Proceso), lo que solicitará al proceso que termine su ejecución de manera suave.

Forzar la terminacion de un proceso
```bash
kill -9 PID_proceso
```

Puedes explorar más comandos tilizando la opción de ayuda de cada comando
```bash
man nombre_comando

nombre_comando --help
```

---

### Utilidades

 El comando tree es una utilidad comúnmente utilizada para visualizar la estructura de directorios de forma jerárquica
 ```bash
 tree
 ```
 Este comando mostrará la estructura de directorios del directorio actual.

 Es probable que tengas que descargar el comando
 ```bash
 sudo apt-get install tree
 ```
 Crear el efecto de "lluvia de caracteres" estilo Matrix, similar al visto en la película "The Matrix". Este comando es una especie de pantalla de inicio interactiva que se ejecuta en la terminal de Unix/Linux.
 ```bash
 cmatrix
 ```
 Es probable que tengas que descargar el comando
 ```bash
 sudo apt-get install cmatrix
 ```

 ---

 ### Editor de texto

 #### nano
 Nano es un editor de texto simple y fácil de usar que es ideal para usuarios principiantes.Tiene una interfaz intuitiva y es más fácil de aprender que Vim o Emacs.

 Para abrir un archivo con Nano, simplemente escribe nano seguido del nombre del archivo en la terminal y presiona Enter. Esto abrirá el archivo en Nano, donde puedes comenzar a editar. Para guardar los cambios y salir, presiona Ctrl + o para guardar y Ctrl + x para salir.
 ```bash
 nano nombre_archivo
 ```