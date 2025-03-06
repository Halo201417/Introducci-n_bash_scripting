# 🚀 Operadores AND y OR  

En este apartado veremos cómo usar estas dos **puertas lógicas** en **Bash**. 🖥️💡  

---  

## 🔗 Operador AND  

El operador `AND` (`&&` en Bash) funciona como **dos puertas**, es decir,  
si **la primera se ejecuta correctamente**, la **segunda también se ejecutará**.  
📌 Es mejor verlo con un ejemplo:  


```bash
ping -c 1 www.google.es && echo "El ping ha finalizado"
```

Si introducimos este código en nuestro script, veremos que después del ping,
se muestra por pantalla el mensaje del `echo`.

💥 Pero si la primera parte falla, la segunda no se ejecutará:

Pero si hacemos a proposito que falle la primera parte la segunda no se ejecutara

```bash
ping -c 1 www.ggogle.es && echo "El ping ha finalizado"
```
---

## 🔀 Operador OR
El operador `OR` (`||` en Bash) funciona como dos caminos, es decir,
si el primer comando no se ejecuta correctamente, entonces se ejecutará el segundo.

📌 Veámoslo con un ejemplo:

```bash
ping -c 1 wwww.google.es || echo "La direccion no existe"
```

Si ejecutamos este script, podemos observar que si el ping falla,
entonces se ejecutará el `echo` mostrando el mensaje de error.
Pero si la URL es correcta, el `echo` no se ejecutará. ✅

```bash
ping -c 1 wwww.googlre.es || echo "La direccion no existe"
```

¡Ahora ya sabes cómo usar `&&` y `||` en Bash! 🚀🎉

























