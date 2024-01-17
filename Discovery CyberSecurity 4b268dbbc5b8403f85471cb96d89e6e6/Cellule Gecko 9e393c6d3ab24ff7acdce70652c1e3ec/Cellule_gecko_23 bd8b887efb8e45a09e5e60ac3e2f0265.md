# <Cellule_gecko_23>

---

[https://cdn.intra.42.fr/pdf/pdf/120549/en.subject.pdf](https://cdn.intra.42.fr/pdf/pdf/120549/en.subject.pdf)

---

En este caso se nos proporciona una serie de palabras o passwords que serán las que conformen mediante algún tipo combinación (o no) el hash que se nos ha mostrado en el subject.

```jsx
c967d488512ab5559b446f97843de1be0d615088
```

---

Nos introducen a una herramienta llamada “John The Ripper”, sin embargo no se nos permite usarla. Ni ningún programa ejecutable en el ordenador…

Después de una intensa búsqueda frustrante por internet, buscando versiones online, y unos cuantos intentos combinando operadores y hashes en CyberCook, decidí hacer la prueba yo mismo de manera inversa. De manera que empecé a probar combinaciones lógicas de contraseñas y comparar el resultado del hash con el que tenemos en el subject.

---

```jsx
liam
42
barcelona
up2u
1978
lion
spain
hacking
```

---

Hasta que en las primeras comprobaciones de combinaciones lógicas, resultó ser el nombre el usuario de Twitter de los anteriores ejercicios.

![Screen Shot 2024-01-16 at 7.21.19 PM.png](Cellule_gecko_23%20bd8b887efb8e45a09e5e60ac3e2f0265/Screen_Shot_2024-01-16_at_7.21.19_PM.png)

Et voilá, damos por concluido esta discovery de ciberseguridad.

> Flag: 42BCN{liamup2u}
>