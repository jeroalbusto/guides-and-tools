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

## Curl

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

### Comandos Basicos de la Terminal


Mostrar la ruta del directorio actual:
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