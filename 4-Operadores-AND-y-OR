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

Si nosotros introducimos en nuestro script este codigo veremos como despues del ping se muestra por pantalla el echo que hemos realizado.

Pero si hacemos a proposito que falle la primera parte la segunda no se ejecutara

```bash
ping -c 1 www.ggogle.es && echo "El ping ha finalizado"
```
---

## Operador OR

El operador `OR` (`||` en bash) funciona como dos caminos, es decir, si no se ejecuta uno
se ejecuta el otro, al igual que con AND es mejor verlo con un ejemplo.

```bash
ping -c 1 wwww.google.es || echo "La direccion no existe"
```

Si ejecutamos este script podemos observar que se realizara el ping pero no el echo. Pero si ponemos mal nuestra
URL vemos que si se ejecuta el echo que hemos escrito.





























