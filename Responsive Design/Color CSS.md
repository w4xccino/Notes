## **Aprende sobre colores complementarios**

La teoría del color y su impacto en el diseño es un tema pesado y solo cubriremos los aspectos básicos en los próximos desafíos. En un sitio web, los colores llaman la atención, provocan emociones y crean una armonía visual. Con diferentes combinaciones de colores se puede cambiar el aspecto de un sitio web y requiere una planificación extensa decidirse por una paleta de color que se integre con nuestro contenido.

El círculo cromático es una herramienta útil para observar cómo los colores están relacionados entre sí - es un círculo donde los tonos similares están juntos y los tonos diferentes alejados. Cuando dos colores opuestos están juntos en el círculo, se los llama colores complementarios. Se caracterizan porque si se combinan, se cancelan así mismos y crean un color gris. Sin embargo, al ubicarse juntos, estos colores parecen más brillantes y producen un contraste visual fuerte.

A continuación hay algunos ejemplos de colores con sus códigos hexadecimales:

> rojo (#FF0000) y cian (#00FFFF)  
> verde(#00FF00) y magenta (#FF00FF)  
> azul (#0000FF) y amarillo (#FFFF00)

Esto es diferente del anticuado modelo de color RYB que muchos de nosotros aprendimos en la escuela, que tiene diferentes colores primarios y complementarios. La teoría moderna del color utiliza el modelo aditivo RGB (como en una pantalla de computadora) y el modelo restante CMY(K) (como en la impresión). Lee [aquí](https://en.wikipedia.org/wiki/Color_model) para obtener más información sobre este complejo tema.

Hay muchas herramientas de selección de color disponibles en línea que tienen la opción de encontrar el complemento de un color.

**Nota:** El uso del color puede ser una forma poderosa de agregar interés visual a una página. Sin embargo, el color por sí solo no debe utilizarse como la única manera de transmitir información importante porque los usuarios con deficiencias visuales pueden no entender ese contenido. Esta cuestión se tratará con más detalle en los desafíos de accesibilidad aplicada.

# **Aprende sobre colores terciarios**

Los monitores y las pantallas crean diferentes colores al combinar cantidades de luz roja, verde y azul. Esto se conoce como modelo aditivo de color RGB en la teoría de moderna de color. Rojo (R), verde (G) y azul (B) «por sus siglas en inglés» son colores primarios. Al combinar dos colores primarios se los colores secundarios cian (G + B), magenta (R + B) y amarillo (R + G). Ya viste estos colores en los desafíos de colores complementarios. Estos colores secundarios son el complemento del color primario no utilizado en su creación y están frente a ese color primario en el círculo cromático. Por ejemplo, el magenta está compuesto de rojo y azul y es el complemento del verde.

Los colores terciarios se forman al combinar dos colores primarios con uno de sus vecinos de color secundario. Por ejemplo, entre el modelo de color RGB, rojo (primario) y amarillo (secundario) forman naranja (terciario). Esto añade seis colores a un círculo cromático simple para un total de doce.

Hay varios métodos para seleccionar colores diferentes que resultan de una combinación armoniosa en diseño. Un ejemplo que puede usar colores terciarios es el esquema de color complementario dividido. Este esquema comienza con un color base, luego lo empareja con los dos colores que están adyacentes a su complemento. Los tres colores proporcionan un fuerte contraste visual en un diseño, pero son más sutiles que utilizar dos colores complementarios.

Aquí hay tres colores creados usando el esquema de dividir-complemento:


| Color | Código hexadecimal |
|--------|---------------------|
| anaranjado| #FF7F00|
|cian | #00FFFF|
|frambuesa| #FF007F|

### MATIZ
En CSS el matiz se representa con la funcion hsl()
- hue
- saturation
- lightness

**Ejemplo**
```css
hsl(180,90%,85%)
```

# **Crea un gradiente lineal de CSS gradual**

La aplicación de un color en elementos HTML no se limita a un tono plano. CSS proporciona la capacidad de usar transiciones de color, también conocidas como degradados, en los elementos. Esto se accede a través de la función `linear-gradient()` de la propiedad `background`. Aquí está la sintaxis general:

```css
background: linear-gradient(gradient_direction, color 1, color 2, color 3, ...);
```

El primer argumento especifica la dirección desde la que comienza la transición de color, se puede establecer como un grado, donde `90deg` hace un gradiente horizontal (de izquierda a derecha) y `45deg` hace un gradiente diagonal (de abajo a izquierda hacia arriba a la derecha). Los siguientes argumentos especifican el orden de los colores utilizados en el degradado.

Ejemplo:

```css
background: linear-gradient(90deg, red, yellow, rgb(204, 204, 255));
```