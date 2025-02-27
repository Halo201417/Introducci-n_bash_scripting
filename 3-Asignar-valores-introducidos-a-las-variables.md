# 📝 Asignar valores introducidos a las variables

Una vez vista la declaración de las variables, ampliaremos cómo manejarlas para que el usuario pueda interactuar con el shell. Veremos cómo los `input` pueden realizarse de varias maneras diferentes. 🎯

---

## ⌨️ Asignación por parte del usuario en Shell
Esta es una de las formas menos comunes para permitir al usuario declarar una variable. Primero, en la declaración dentro de nuestro script, la igualaremos con la siguiente instrucción `$n`, siendo `n` un número que empieza desde `1` hasta `n` variables de este tipo. 🔢

```bash
variable1=$1
variable2=$2
# Para imprimir cualquier variable usaremos el comando echo acompañado del simbolo $
echo $variable1 $variable2
```

Una vez creadas nuestras variables, podemos asignar cualquier valor que deseemos a nuestras variables.

```bash
[alumno@debian:~]$ ./prueba.sh 7 "Hola"
7 Hola
```

---

## 🛠️ Asignanción por parte del usuario en ejecución

Se nos puede presentar la ocasión en la que el usuario, por cualquier motivo, necesite introducir un carácter o número en medio de la ejecución de nuestro script. Un ejemplo claro es cuando realizamos una instalación o actualización del sistema y nos pide confirmación. ✅

Para esta acción, usaremos la función `read -p`, la cual nos permite pedirle al usuario que introduzca un valor en la variable. 📝

```bash
read -p "Introduzca su nombre: " nombre
read -p "Introduzca su edad: " edad

echo "El nombre del usuario es $nombre y tiene $edad años"
```

Ejemplo de ejecución:

```bash
[alumno@debian:~]$ ./prueba.sh
Introduzca su nombre: Alumno
Introduzca su edad: 120
El nombre del usuario es Alumno y tiene 120 años
```

🚀 ¡Ahora ya sabes cómo asignar valores a variables en Bash! 🏆
