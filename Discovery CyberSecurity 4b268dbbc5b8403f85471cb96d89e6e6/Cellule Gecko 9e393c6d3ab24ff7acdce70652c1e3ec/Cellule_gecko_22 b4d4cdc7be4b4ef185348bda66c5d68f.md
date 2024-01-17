# <Cellule_gecko_22>

---

[https://cdn.intra.42.fr/pdf/pdf/120546/en.subject.pdf](https://cdn.intra.42.fr/pdf/pdf/120546/en.subject.pdf)

---

Esta vez, no tendremos que desencriptar, sino decodificar un hash.

```jsx
629cf0d815ccb448a2c7a4d3d9cc3989
```

---

<aside>
💡 **Hashcat** 
Es una herramienta para recuperación de contraseñas. Tuvo su base de código propietario hasta 2015, pero luego fue liberada como software de código abierto. Hay versiones disponibles para Linux, macOS y Windows. Algunos ejemplos de algoritmos hash compatibles con Hashcat son los hashes LM, [MD4](https://es.wikipedia.org/wiki/MD4), [MD5](https://es.wikipedia.org/wiki/MD5), varios tipos de SHA y los formatos crypt (Unix), así como los algoritmos utilizados en [MySQL](https://es.wikipedia.org/wiki/MySQL) y [Cisco PIX](https://es.wikipedia.org/wiki/Private_Internet_Exchange).

</aside>

---

Vamos a tener que descubrir que algortimo de encriptación tiene nuestro hash. Despues de un par de prubas, comenzando por por los mas comunos, descubriremos que se trata de MD5, ya que nos devuelve una palabra española con sentido:

[MD5 Encrypt/Decrypt Online | 10015 Tools](https://10015.io/tools/md5-encrypt-decrypt)

![Screen Shot 2024-01-16 at 6.26.55 PM.png](Cellule_gecko_22%20b4d4cdc7be4b4ef185348bda66c5d68f/Screen_Shot_2024-01-16_at_6.26.55_PM.png)

---

> Flag: 42BCN{palito}
>