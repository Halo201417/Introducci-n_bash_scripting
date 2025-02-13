# 📄 Cómo hacer un archivo `.sh`

En esta primera parte, veremos cómo crear un archivo ejecutable en Bash. Como se mencionó en el README, se utilizará principalmente la herramienta **nano** para crear y modificar el archivo. Sin embargo, esto no limita el uso de otros editores mencionados o incluso otros que no se hayan incluido como ejemplo.

---

## 🛠️ Creación del archivo

Para crear un archivo, debemos usar el comando `sudo` o estar como **root** del sistema.

```bash
[alumno@debian:~]$ sudo nano script.sh
```

Escribiremos dentro del archivo el siguiente código para realizar una prueba:

```bash
echo "Hola Mundo"
```

Guardaremos el archivo con la combinación `Ctrl + O` y saldremos con `Ctrl + x`.

Después de crear el archivo, podemos usar el comando ls para comprobar que ha sido creado. Sin embargo, observaremos que no tiene ningún tipo de color, lo que significa que no tiene permisos de ejecución.

---

## 🔒 Asignar permisos a nuestro archivo

Para asignar permisos de ejecución, utilizaremos el comando `chmod`.

```bash
[alumno@debian:~]$ sudo chmod +x script.sh
```

Ahora, si ejecutamos `ls`, veremos que nuestro archivo está en verde, lo que indica que está listo para ser ejecutado.

--- 

## 🚀 Ejecutar nuestro archivo

Podemos ejecutar nuestro archivo de dos maneras:

1. Llamando al tipo de archivo:

```bash
[alumno@debian:~]$ sh ./script.sh
```

2. Directamente llamando al archivo:

```bash
[alumno@debian:~]$ ./script.sh
```

---

¡Y eso es todo! Ahora has creado, asignado permisos y ejecutado tu primer script en Bash. 🎉
