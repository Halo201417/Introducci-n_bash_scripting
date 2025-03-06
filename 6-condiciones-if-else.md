# ⚡ Condiciones en Bash (`if-else`)  

En este apartado aprenderemos sobre las **condiciones en Bash**, similares a las que existen en otros lenguajes como **C**.  
En concreto, veremos el uso de `if-else`. 🖥️💡  

---  

## 🔢 Operadores y estructura básica  

Si vienes de otros lenguajes de programación, podrías pensar que los operadores dentro de los condicionales son iguales.  
Tienes razón en parte, ya que algunos operadores como `==`, `!=`, `<=`, etc., son similares.  

📌 **Pero en Bash, para comparar números y salidas, se utilizan operadores específicos:**  

| Operador  | Significado          |
|-----------|----------------------|
| `-gt`     | Mayor que (`>`)      |
| `-lt`     | Menor que (`<`)      |
| `-ge`     | Mayor o igual (`>=`) |
| `-le`     | Menor o igual (`<=`) |
| `-eq`     | Igual que (`==`)     |
| `-ne`     | Distinto que (`!=`)  |

Ahora que conocemos los operadores, veamos un **ejemplo práctico**:  

```bash
variable1=10
variable2=10

if test $variable1 -eq $variable2; then
        echo "Las variables son iguales"
else 
        echo "La variable 2 es mayor"
fi
```

📌 Explicación del código

1️⃣ Definimos dos variables numéricas, variable1 y variable2.

2️⃣ Utilizamos if test $variable1 -eq $variable2; para comparar los valores.
test es un comando en Bash que evalúa expresiones.
-eq significa "igual que", por lo que estamos comprobando si variable1 es igual a variable2.

3️⃣ Si la condición es verdadera (true), se ejecutará el bloque dentro del then, mostrando el mensaje "Las variables son iguales".

4️⃣ Si la condición es falsa (false), se ejecutará el bloque dentro del else, mostrando "La variable 2 es mayor".

5️⃣ Finalizamos la estructura con fi, que cierra el if.

---

## 🔍 Inspección de archivos en Bash  

El siguiente script recorre todos los archivos en el directorio actual y, si encuentra el archivo `script.sh`, lo muestra por pantalla. 

```bash
for i in *; do
    if [ "$i" = "script.sh" ]; then
        echo "Inspeccionamos el archivo $i"
        cat "$i"
    else
        echo "No se inspecciona el archivo $i"
    fi
done
```

📖 Explicación del código

1️⃣ El bucle for recorre todos los archivos (*) en el directorio actual.

2️⃣ La condición if [ "$i" = "script.sh" ]; then verifica si el archivo actual ($i) es script.sh.

> [!WARNING]
> En Bash, para comparar cadenas se usa [ "$var" = "valor" ], no test $var = "valor".

3️⃣ Si el archivo es script.sh, se imprime un mensaje y se muestra su contenido con cat.

4️⃣ Si el archivo es otro, se imprime un mensaje indicando que no se inspeccionará.

5️⃣ Finalizamos el if con fi y el for con done.

---

¡Así de fácil es recorrer archivos y aplicar condiciones en Bash! 🚀😃


























