# Git

Git es un software de control de versiones, que te permite trabajar en equipo, y tener un control de tu codigo y las versiones del mismo

## Instalacion

Para instalar git en linux lo podes hacer con el comando:
```bash
sudo apt-get install git
```

para ver si esta instalado git usa el comando:
```bash
git --version
```
esto te mostrara la version de git que tenes instalada, por ende quiere decir que tenes git instalado

---

### configuración básica

Configurar Nombre que salen en los commits:
```bash
git config --global user.name "name_ejemplo"
```
Configurar Email:
```bash
git config --global user.email name_ejemplo@gmail.com
```

---

### comandos basicos

Iniciamos GIT en la carpeta donde esta el proyecto con el comando:
```bash
git init
```

Clonamos un repositorio de github o gitlab:
```bash
git clone <url>
```

Lista un estado actual del repositorio con lista de archivos modificados o agregados:
```bash
git status
```

Añadimos todos los archivos para el commit:
```bash
git add .
```

Hacemos el primer commit:
```bash
git commit -m "Texto que identifique el cambio que se realizo"
```

Subimos al repositorio:
```bash
git push -u origin master
```

---

### git add

Añadimos un archivo para el commit:
```bash
git add <archivo>
```
Añadimos todos los archivos con la extensión especificada:
```bash
git add *.txt
```

---

### git push

Subimos al repositorio:
```bash
git push origin <rama>
```

---

### git log
Muestra los logs de los commits:
```bash
git log
```
Muestras los cambios en los commits:
```bash
git log --oneline --stat
```
Muestra graficos de los commits:
```bash
git log --oneline --graph
```

---