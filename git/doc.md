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

### git branch

Crear un branch o rama:
```bash
git branch <name_Branch>
```
Lista los branches o ramas:
```bash
git branch
```
Comando -d elimina el branch y lo une al master:
```bash
git branch -d <name_Branch>
```
Elimina sin preguntar branch:
```bash
git branch -D <name_Branch>
```

---

### git checkout

cambiar de branch o rama:
```bash
git checkout <name_branch>
```
Crear una nueva rama y cambiar a ella:
```bash
git checkout -b <name_branch>
```

---

### otros comandos

Une el branch actual con el especificado:
```bash
git merge <name_Branch>
```
se utiliza para fusionar cambios de una rama a otra en Git. Básicamente, toma los cambios que se han realizado en una rama y los integra en otra rama.es una operación fundamental en Git y se utiliza comúnmente para integrar cambios de diferentes ramas, como por ejemplo, fusionar una rama de características con la rama principal del proyecto.



Verifica cambios en el repositorio online o remoto con el local:
```bash
git fetch <repositorio_remoto>
```
este comando recupera todo del repositorio remoto que aún no están presentes en tu repositorio local. Sin embargo, no realiza una fusión (merge) de estos cambios con tus ramas locales ni modifica tu directorio de trabajo.Esto significa que puedes inspeccionar los cambios antes de fusionarlos, lo que te permite revisar los cambios antes de incorporarlos a tu rama local.

Busca los cambios nuevos y actualiza el repositorio:
```bash
git pull origin <name_Branch>
```
se utiliza para recuperar los cambios desde un repositorio remoto y fusionarlos con la rama local actual. Básicamente, realiza dos operaciones en una sola (git fetch, git merge).
Es útil para mantener tu repositorio local actualizado con los últimos cambios realizados en el repositorio remoto y para sincronizar tu trabajo con el de otros colaboradores del proyecto.