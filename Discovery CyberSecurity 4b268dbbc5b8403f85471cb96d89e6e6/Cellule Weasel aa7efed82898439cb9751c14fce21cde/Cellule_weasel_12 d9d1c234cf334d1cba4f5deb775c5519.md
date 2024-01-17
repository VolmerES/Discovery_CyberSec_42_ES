# <Cellule_weasel_12>

---

[https://cdn.intra.42.fr/pdf/pdf/120534/en.subject.pdf](https://cdn.intra.42.fr/pdf/pdf/120534/en.subject.pdf)

---

Para este utilizaremos un metodo llamado Path traversal, como nos sugiere el subject:

<aside>
💡 **PATH TRAVERSAL**

Un **directory traversal** (o **salto de directorio** o **cruce de directorio** o **path traversal**) consiste en explotar una vulnerabilidad informática que ocurre cuando no existe suficiente seguridad en cuanto a la validación de un usuario, permitiéndole acceder a cualquier tipo de directorio superior (padre) sin ningún control.

La finalidad de este ataque es ordenar a la aplicación a acceder a un [archivo](https://es.wikipedia.org/wiki/Archivo_(computaci%C3%B3n)) al que no debería poder acceder o no debería ser accesible. Este ataque se basa en la falta de seguridad en el código. El software está actuando exactamente como debe actuar y en este caso el atacante no está aprovechando un [bug](https://es.wikipedia.org/wiki/Error_de_software) en el código.

**Directory traversal** también es conocido como el ../ ataque punto punto barra, escalado de directorios y backtracking.

</aside>

---

La pagina sería la siguiente:

![Screen Shot 2024-01-16 at 3.26.14 PM.png](Cellule_weasel_12%20d9d1c234cf334d1cba4f5deb775c5519/Screen_Shot_2024-01-16_at_3.26.14_PM.png)

---

Buscando a con path traversal, se encontro una ruta con lo usuarios:

![Screen Shot 2024-01-16 at 3.27.02 PM.png](Cellule_weasel_12%20d9d1c234cf334d1cba4f5deb775c5519/Screen_Shot_2024-01-16_at_3.27.02_PM.png)

![Screen Shot 2024-01-16 at 3.27.28 PM.png](Cellule_weasel_12%20d9d1c234cf334d1cba4f5deb775c5519/Screen_Shot_2024-01-16_at_3.27.28_PM.png)

---

La solución resultó ser mas sencilla de lo esperado:

![Screen Shot 2024-01-16 at 4.06.10 PM.png](Cellule_weasel_12%20d9d1c234cf334d1cba4f5deb775c5519/Screen_Shot_2024-01-16_at_4.06.10_PM.png)

Encontrando el siguiente resultado:

![Screen Shot 2024-01-16 at 3.26.30 PM.png](Cellule_weasel_12%20d9d1c234cf334d1cba4f5deb775c5519/Screen_Shot_2024-01-16_at_3.26.30_PM.png)

---

> Flag: 42BCN{p47h7r4v3rs4l1s7h3w4y}
>