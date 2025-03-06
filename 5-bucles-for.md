# 🔄 Bucle `for` en Bash  

En este apartado aprenderemos sobre el **bucle `for`** en **Bash** y veremos qué podemos hacer con él. 🖥️💡  

---  

## 📌 Estructura básica  

Un **bucle `for`** en Bash sigue siempre la misma estructura: 

```bash
for i in alumno profesor deberes; do
        echo "El valor de i en esta vuelta es $i"
done
```

Vamos a explicar paso a paso qué ocurre aquí:

1️⃣ Declaramos el bucle `for` y una variable (`i`) que almacenará los valores que recorreremos en el bucle.

2️⃣ La palabra clave `in` indica que iteraremos sobre un conjunto de elementos (puede ser una lista, archivos, directorios, etc.).
    En este caso, recorremos una lista de cadenas de texto.
    
3️⃣ El `do` señala el inicio del bloque de instrucciones que se ejecutará en cada iteración.

4️⃣ Dentro del bucle, imprimimos cada elemento de la lista.

5️⃣ Finalizamos el bucle con `done`, indicando que hemos terminado.

🔹 ¡Así de simple! Esta es la estructura más básica de un bucle `for` en Bash.

---

📂 Ejemplo: Listar archivos
Supongamos que tenemos muchos archivos en un directorio y queremos ejecutar un script que imprima sus nombres en pantalla.
Podemos usar el carácter `*` para recorrer todos los archivos del directorio actual.

```bash
for i in *; do
        echo "En esta vuelta, tengo seleccionado el archivo $i"
done
```

📌 ¿Qué hace `*`?
El `*` representa todos los archivos en el directorio actual, por lo que el bucle iterará sobre cada uno de ellos.

---

¡Ahora ya sabes cómo utilizar el bucle `for` en Bash! 🚀🎉






















