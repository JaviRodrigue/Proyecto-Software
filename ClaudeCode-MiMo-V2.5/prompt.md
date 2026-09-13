# Enunciado 5

Tenemos que generar un **sitio web estático (sin scripts)** que permita difundir un emprendimiento en el cual vendemos artesanías agrupados por categorías: 
- **tejidos** 
- **cerámicas**
- **pinturas**.

La información a mostrar por cada artículo está en un directorio denominado **“artículos”** y dentro de éste, tres directorios, uno por categoría de artículos.

Por cada artículo a mostrar en la página, hay dos archivos: uno denominado **“articulo1.png”** que corresponde a una imagen representativa del artículo y otro denominado **“articulo1.pdf”** con información adicional del producto.
en la carpeta imagenes, estan las imagenes, con sus nombre correspondiente para las categorias.
siguiendo las intrucciones anteriores, crea un archivo.pdf para cada imagen, y esten ordenadas como anteriormente se menciono
```text
Opencode-DeepSeek-V4/
├── index.html
├── estilosIA.css
└── articulos/
    ├── tejidos/
    │   ├── tejido1.png
    │   ├── tejido1.pdf
    │   ├── tejido2.png
    │   ├── tejido2.pdf
    │   ├── tejido3.png
    │   └── tejido3.pdf
    ├── ceramicas/
    │   ├── ceramica1.png
    │   ├── ceramica1.pdf
    │   ├── ceramica2.png
    │   ├── ceramica2.pdf
    │   ├── ceramica3.png
    │   └── ceramica3.pdf
    └── pinturas/
        ├── pintura1.png
        ├── pintura1.pdf
        ├── pintura2.png
        ├── pintura2.pdf
        ├── pintura3.png
        └── pintura3.pdf
```


Por ejemplo, para la categoría **tejidos** se podría mostrar algo similar a:

- Una imagen representativa del artículo.
- Un borde alrededor de la tarjeta.
- Relleno (*padding*) dentro de la tarjeta.
- Un enlace o botón **“+ Info”** para acceder a la información adicional. al presionar el "+ Info", le debera mostrar la informacion que se encuentra en el archivo.pdf correspondiente de la imagen dada. Por ejemplo, si presiona el de tejido1.png, debera de mostrar la informacion que se encuentra en tejido1.pdf

## Condiciones del sitio

1. Se debe mostrar una **barra de navegación** (dispuesta como más les guste) con enlaces a:
   - **Información de contacto:** un formulario simple con los datos que les parezcan más adecuados para esta sección. En la informacion de contacto, quiero que se contemple lo siguiente
     - Nombre completo (requerido)
     - correo electronico (requerido)
     - Mensaje (requerido)
   - **Información de quien mantiene el sitio.**: para este apartado quiero que agregues mi informacion basica
     - Acerca del proyecto: "Este sitio web fue creado como parte de una actividad academica de la materia "Proyecto de Software" y el objetivo de la pagina
     - informacion del autor
       - mi nombre: Javier Rodriguez
       - correo: agudtinjava@gmail.com
       - software developer
       - con un boton de contactar que redirija al inciso anterior
     - tecnologias usadas:
       - HTML5 semantica
       - CSS3 con diseño responsive
     - utlima actualizacion, con la fecha de la ultima actualizacion
   - **Lista de artículos agrupados por categorías.**, las categorias se mencionaron anteriormente 

2. Pueden indicar los **colores y estilos** que prefieran. es requerido usar contrastes de color adecuado entre texto y fondo

3. Respecto a la interacción con el sitio, se debe poder **elegir una categoría** (ya sea desde una lista de opciones desplegable, *radio buttons* o la opción que prefieran) y, al seleccionar dicha categoría, mostrar los artículos con la información asociada, como se muestra en la imagen. para este caso quiero que se use una lista de opciones despegable

   **Siempre en forma estática.**

4. El sitio debe ser **responsivo**. quiero que uses @media queries, unidades relativas

5. Solo se debe usar **HTML y CSS**. no se debe de utilizar nada de script ni de Js, ni tampoco se puede utilizar frameworks

6. Las reglas de estilo deben estar en un **archivo separado** denominado `estilosIA.css`. no puede haber estilos en los HTML

7. Se debe trabajar con información de **al menos 3 artículos por cada categoría** a mostrar.

8. debe tener los tags semanticos bien defenidos (<header><main><footer><nav><article>). Tambien los "Meta Tags", describirlo adecuadamente los metadatos de las paginas (codificacion de caracteres, adaptabilidad y descripcion).
9. la pagina estatica debe ser accecible desde el lector de pantalla y tambien realizar la navegacion utilizando unicamente el teclado, teniendo en cuenta que tiene que ser logico el orden de anuncio de los elementos de la pagina
10. tenes que proveer equivalentes textuales para contenidos no textual (Imagenes, audios, videos)

---

## Información de los artículos

Cada artículo del catálogo se muestra con el nombre y la descripción que se detallan a continuación, agrupados por categoría.

### Tejidos

| Imagen | Nombre | Descripción |
| :--- | :--- | :--- |
| tejido1.png | Dos patitos | Tejido a mano en lana de dos patitos. |
| tejido2.png | Tejido de Tom Lagartija | Tejido a mano en lana de tom lagartija de Hoppers. |
| tejido3.png | Tejido de Ratatouille | Tejido a mano en lana de ratatouille. |

### Cerámicas

| Imagen | Nombre | Descripción |
| :--- | :--- | :--- |
| ceramica1.png | Taza de paisaje | Taza de cerámica de paisaje en las montañas. |
| ceramica2.png | Taza de ovejas | Taza de cerámica de paisaje con ovejas. |
| ceramica3.png | Taza de patos | Plato decorativo de cerámica de dos patos. |

### Pinturas

| Imagen | Nombre | Descripción |
| :--- | :--- | :--- |
| pintura1.png | Cuadro al Óleo | Paisaje original al óleo con pastas que capturan la luz, que representa la puerta de una oportunidad. |
| pintura2.png | Acuarela Río | Cuadro de la noche estrellada de Van Gogh, pintado en acuarela sobre papel de algodón. |
| pintura3.png | Atardecer al Pastel | Obra del El Principito, con colores pastel y un cielo estrellado. |

## Información de los PDF

Cada archivo PDF (asociado por nombre a su imagen) es la ficha del producto e incluye: **Categoría, Código, Nombre, Descripción, Materiales, Medidas y Precio sugerido**.

| Código | Materiales | Medidas | Precio sugerido |
| :--- | :--- | :--- | :--- |
| tejido1 | Lana acrílica suave, ojos de seguridad, relleno sintético hipoalergénico. | Aprox. 12 cm de alto cada patito. | $9.500 |
| tejido2 | Lana de algodón, ojos de seguridad plásticos, relleno hipoalergénico. | Aprox. 20 cm de largo. | $12.800 |
| tejido3 | Lana acrílica con detalles tejidos en aguja, relleno sintético. | Aprox. 15 cm de alto. | $13.500 |
| ceramica1 | Arcilla de gres esmaltada, esmalte atóxico para alimentos. | Capacidad aprox. 250 ml. | $14.900 |
| ceramica2 | Gres esmaltado, decoración pintada a mano. | Capacidad aprox. 250 ml. | $15.400 |
| ceramica3 | Arcilla blanca esmaltada, decoración pintada a mano. | Diámetro aprox. 20 cm. | $11.900 |
| pintura1 | Óleo sobre lienzo de algodón, bastidor de madera. | 60 x 80 cm. | $58.000 |
| pintura2 | Acuarela sobre papel de algodón. | 30 x 40 cm. | $21.700 |
| pintura3 | Pastel seco sobre papel texturado con fijador. | 45 x 60 cm. | $33.500 |