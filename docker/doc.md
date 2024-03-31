# docker - compose

Docker Compose es una herramienta que se utiliza para definir y ejecutar aplicaciones Docker de múltiples contenedores. Permite definir la configuración de la aplicación en un archivo .YAML y luego utilizar un conjunto de comandos para gestionar esos contenedores

## Instalación

docker-compose se puede instalar en linux con el comando:
```bash
sudo apt-get install docker-compose
```

para verificar si esta instalado, usa el comando:
```bash
docker-compose -v
```
o
```bash
docker-compose --version
```
esto te dira la version de docker-compose que instalastes

---

### comandos basicos

Para crear e iniciar los contenedores definidos en el archivo docker-compose.yml se usa:
```bash
sudo docker-compose up
```
para usarlo en modo detach
```bash
sudo docker-compose up -d
```

Para detener y elimina los contenedores definidos en el archivo docker-compose.yml se usa:
```bash
sudo docker-compose down
```

Para construir o reconstruir los contenedores definidos en el archivo docker-compose.yml. Se usa cuando se realizan cambios en el código o en la configuración del contenedor y se desea reconstruir las imágenes. Usa el comando:
```bash
sudo docker-compose build
```

Para iniciar los contenedores definidos en el archivo docker-compose.yml, pero no los crea si no existen. Se usa:
```bash
sudo docker-compose start
```

Para detener los contenedores definidos en el archivo docker-compose.yml, pero no los elimina. Se usa:
```bash
sudo docker-compose stop
```

Para reiniciar los contenedores definidos en el archivo docker-compose.yml. Se usa:
```bash
sudo docker-compose restart
```

Para mostrar el estado y los contenedores funcionando,y definidos en el archivo docker-compose.yml. Se usa:
```bash
sudo docker-compose ps
```
Para mostrar el estado y los contenedores que creastes, se usa:
```bash
sudo docker-compose ps -a
```
Para mostrar los logs de los contenedores definidos en el archivo docker-compose.yml. Se usa:
```bash
sudo docker-compose logs
```

---

### comandos de docker
