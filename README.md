# Aprendiendo la Terminal de Linux

> "El conocimiento es poder, y el poder... se ejecuta con sudo."

---

## 🧭 Introducción

### 🐧 ¿Cómo nació Linux?

Linux nació en **1991**, cuando **Linus Torvalds**, un joven estudiante finlandés, decidió crear su propio sistema operativo inspirado en UNIX. Su idea inicial era simplemente aprender más sobre cómo funcionaban los sistemas, pero terminó iniciando una revolución en el mundo del software. Así nació el núcleo (*kernel*) de Linux, que más tarde se combinaría con herramientas del proyecto GNU para formar los sistemas que conocemos hoy.

### 💡 Filosofía de Linux

La filosofía de Linux se basa en tres pilares fundamentales: **libertad, colaboración y conocimiento compartido**. Es un sistema **de código abierto**, lo que significa que cualquiera puede estudiar, modificar y mejorar su funcionamiento. Esta mentalidad ha permitido que Linux evolucione gracias al esfuerzo conjunto de millones de desarrolladores en todo el mundo.

Hoy, la mayoría de los **servidores del mundo** funcionan con Linux, y la mayor parte de su administración se realiza desde la **terminal**, el corazón del sistema y símbolo de su eficiencia.

Aprender a usar la terminal no solo te da control absoluto sobre tu sistema, sino que también te enseña a pensar como un verdadero ingeniero.

---

## ⚙️ Comandos Básicos

### 🔐 Cambiar a modo superusuario

```bash
sudo su
```

Permite ejecutar comandos con privilegios de administrador.

> Usa este comando con precaución: un error puede romper el sistema más rápido que un *error capa 8* con café derramado.

### 🔄 Actualizar el sistema

```bash
sudo apt update && sudo apt upgrade
```

`update` actualiza la lista de paquetes disponibles, y `upgrade` instala las versiones más recientes.

---

## 📦 Instalación y Desinstalación de Programas

### 🧩 Instalar desde repositorios

```bash
sudo apt install nombre_del_paquete
```

Ejemplo:

```bash
sudo apt install neofetch
sudo apt install htop
```

### 🚀 Instalar con Snap

```bash
sudo snap install nombre_del_paquete
```

Ejemplo:

```bash
sudo snap install code --classic
sudo snap install spotify
```

### 📁 Instalar un paquete .deb

```bash
sudo dpkg -i nombre_del_paquete.deb
```

### ❌ Desinstalar programas

```bash
sudo apt remove nombre_del_paquete
sudo snap remove nombre_del_paquete
```

---

## 📂 Navegación

* `pwd` → Muestra en qué carpeta estás.
* `ls` → Lista los archivos de la carpeta actual.
* `cd nombre_carpeta` → Cambia de carpeta.
* `cd ..` → Sube un nivel.

---

## 🧱 Gestión de Archivos y Carpetas

* `mkdir nombre_carpeta` → Crea una nueva carpeta.
* `rmdir nombre_carpeta` → Elimina una carpeta vacía.
* `rm nombre_archivo` → Elimina un archivo.
* `cp origen destino` → Copia archivos o carpetas.
* `mv origen destino` → Mueve o renombra archivos.

### ⚠️ Comando peligroso: `rm -rf`

```bash
rm -rf nombre_carpeta
```

Elimina una carpeta y **todo su contenido de forma recursiva y sin confirmación**.

> Úsalo con extremo cuidado. Un `rm -rf /` podría borrar todo el sistema operativo. Considera este comando el equivalente a pulsar el botón de autodestrucción del laboratorio de Stark.

---

## 📝 Crear y editar archivos de texto

### Crear un archivo vacío

```bash
touch archivo.txt
```

### Editar un archivo con Nano

```bash
nano archivo.txt
```

* Escribe tu contenido.
* Guarda con **Ctrl + O**, presiona **Enter**.
* Sal con **Ctrl + X**.

---

## ☕ Conclusión

Dominar la terminal de Linux es dominar la base de la infraestructura digital moderna. Todo gran sistema, desde servidores hasta naves espaciales (*guiño, Tony Stark*), necesita un operador que entienda la línea de comandos.

> “El buen código es como un buen espresso: concentrado, potente y mejor si se sirve caliente.”
> — *J.A.R.V.I.S., asistente personal de Faragon*

