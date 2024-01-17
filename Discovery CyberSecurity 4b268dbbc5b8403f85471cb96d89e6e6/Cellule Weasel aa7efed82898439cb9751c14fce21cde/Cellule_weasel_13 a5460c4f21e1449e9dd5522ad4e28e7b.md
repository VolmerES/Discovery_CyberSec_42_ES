# <Cellule_weasel_13>

---

[https://cdn.intra.42.fr/pdf/pdf/120537/en.subject.pdf](https://cdn.intra.42.fr/pdf/pdf/120537/en.subject.pdf)

---

Al acceder a la pagina web encontraremos lo siguiente

![Screen Shot 2024-01-16 at 4.14.10 PM.png](Cellule_weasel_13%20a5460c4f21e1449e9dd5522ad4e28e7b/Screen_Shot_2024-01-16_at_4.14.10_PM.png)

---

<aside>
💡 **Inyección SQL**

Es un método de infiltración de código intruso que se vale de una [vulnerabilidad informática](https://es.wikipedia.org/wiki/Error_de_software) presente en una aplicación en el nivel de validación de las entradas para realizar operaciones sobre una [base de datos](https://es.wikipedia.org/wiki/Base_de_datos).[1](https://es.wikipedia.org/wiki/Inyecci%C3%B3n_SQL#cite_note-1)

El origen de la vulnerabilidad radica en la incorrecta comprobación o filtrado de las variables utilizadas en un programa que contiene, o bien genera, código [SQL](https://es.wikipedia.org/wiki/SQL). Es, de hecho, un error de una clase más general de vulnerabilidades que puede ocurrir en cualquier [lenguaje de programación](https://es.wikipedia.org/wiki/Lenguaje_de_programaci%C3%B3n) o [script](https://es.wikipedia.org/wiki/Lenguaje_interpretado) que esté incrustado en otro.

Se conoce como Inyección SQL, indistintamente, al tipo de vulnerabilidad, al método de infiltración, al hecho de incrustar código SQL intruso y a la porción de código incrustado.

</aside>

---

En este caso, resolveremos la flag con una inyección SQL básica:

![Screen Shot 2024-01-16 at 4.40.19 PM.png](Cellule_weasel_13%20a5460c4f21e1449e9dd5522ad4e28e7b/Screen_Shot_2024-01-16_at_4.40.19_PM.png)

---

Para entender este metodo es interesante leer este enlace:

[Inyección SQL: Guía Detallada para Usuarios de WordPress](https://kinsta.com/es/blog/inyeccion-sql/)

<aside>
💡 Primer elemento:  ‘
La comilla simple terminará la busqueda de usuario en la base de datos sql, de manera que lo pasará por alto a la hora de autentificarse.

</aside>

```jsx
select * from user_table
where username = 'sdaityari'. // Esta es la comilla a la que nos referimos;
and password = 'mypassword';
```

---

<aside>
💡 Segundo element: OR
Este segundo elemento OR, se trata de un operador lógico que nos devolverá 1 en base a la ecuación siguiente 1=1, para entender esto es importante conocer sobre operadores binarios. El resultado final de todo esto será siempre 1, de manera que hará un bypass sobre la contraseña, ya que aunque la contraseña sea incorrecta, el resultado devuelto si. Esta vulnerabilidad aprovecha que se puedan usar espacios para establecer contraseñas.

</aside>

---

<aside>
💡 Tercer elemento: #
Este elemento dará lugar a que todo lo que vaya después de el este comentado para omitirlo.

</aside>

---

Después de darle a enter, nos mostrará la flag que buscabamos.

![Screen Shot 2024-01-16 at 4.49.00 PM.png](Cellule_weasel_13%20a5460c4f21e1449e9dd5522ad4e28e7b/Screen_Shot_2024-01-16_at_4.49.00_PM.png)

---

> Flag: 42BCN{sql1nj3c710n_n1c3}
>