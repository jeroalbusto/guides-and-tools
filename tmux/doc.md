# tmux

tmux es un programa que se ejecuta en la terminal y es conocido como un multiplexor de terminal, te permite dividir la terminal en horizontal y vertical creando varias terminales en una sola ventana. Es muy util poder trabajar en una sola ventana y tener multiples procesos y programas abierto



## Instalacion

se instala en linux con el comando:


```bash{copy}
sudo apt-get install tmux
```

podemos comprobarlo con el comando:
```bash
tmux -V
```
Si tmux está instalado, verás la versión instalada impresa en la terminal


### Comandos

Se puede iniciar tmux de dos maneras:

- escribiedo tmux en la terminal e inicia una session sin nombre
```bash
 tmux
```
- o escribiedo
```bash
 tmux new -s nombre_session
```
esto iniciará una nueva sesión de tmux con el nombre especificado

---

Listar sesiones existentes de tmux:
```bash
tmux ls
```
esto mostrara una lista de sesiones de tmux existentes

---

Dividir la ventana horizontalmente:
```bash
Ctrl + b  %
```
esto dividira la ventana la ventana actual de tmux en dos paneles horizontales

---

Dividir la ventana verticalmente:
```bash
Ctrl + b  "
```
esto dividira la ventana la ventana actual de tmux en dos paneles verticales

---

Alterar o cambiar entre paneles:
```bash
Ctrl + b arrow_key
```
esto permite cambiar entre los paneles divididos

---

Cerrar un panel o cerrar una session en tmux:
```bash
exit
```
esto cerrará el panel actual en tmux y tambien puedes cerrar la session