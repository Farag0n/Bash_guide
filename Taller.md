# Taller Bash

> “La terminal no muerde... a menos que ejecutes `sudo rm -rf /`.”

---

## Actualizar e instalar

1. **Actualizar el sistema:**

   ```bash
   sudo apt update
   sudo apt upgrade
   ```

2. **Instalar un editor de texto:**

   ```bash
   sudo apt install nano
   ```

---

## Navegar y carpetas

1. **Moverte a la carpeta de Documentos:**

   ```bash
   cd ~/Documentos
   ```

2. **Crear una estructura de carpetas:**

   ```bash
   mkdir -p CarpetaPadre/CarpetaHija
   ```

3. **Verifica que existen:**

   ```bash
   ls
   ```

---

## Archivos

1. **Entrar a la CarpetaHija:**

   ```bash
   cd CarpetaPadre/CarpetaHija
   ```

2. **Crear un archivo con contenido:**

   ```bash
   nano hola_mundo.txt
   ```

   Escribe dentro:

   ```
   ¡Hola Mundo desde la Terminal!
   ```

   Guarda con **Ctrl + O**, presiona **Enter** y sal con **Ctrl + X**.

3. **Mostrar el contenido del archivo:**

   ```bash
   cat hola_mundo.txt
   ```

   *Objetivo:* Verificar el contenido del archivo directamente desde la terminal.

4. **Crear un archivo vacío y una carpeta vacía:**

   ```bash
   touch archivo_vacio.txt
   mkdir carpeta_vacia
   ```

5. **Mostrar el contenido de tu carpeta:**

   ```bash
   ls
   ```

---

## Manipulación y limpieza

1. **Copiar tu archivo “hola_mundo.txt” a la carpeta vacía:**

   ```bash
   cp hola_mundo.txt carpeta_vacia/
   ```

2. **Mover tu archivo copiado a la carpeta padre:**

   ```bash
   mv carpeta_vacia/hola_mundo.txt ../
   ```

   *Objetivo:* Aprender a mover archivos entre carpetas sin duplicarlos.

3. **Renombrar tu archivo vacío:**

   ```bash
   mv archivo_vacio.txt notas.txt
   ```

4. **Visualizar el contenido del archivo movido:**

   ```bash
   cat ../hola_mundo.txt
   ```

   *Objetivo:* Confirmar que el archivo se movió correctamente y sigue siendo accesible.

5. **Eliminar lo que creaste (con precaución):**

   ```bash
   rm notas.txt
   rm -rf carpeta_vacia
   cd ..
   rm -rf CarpetaHija
   ```

   *Objetivo:* Practicar la gestión de archivos, el movimiento de datos y el uso responsable del comando `rm -rf`.
