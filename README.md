# Frontend Developer

# HTML

HTML (HyperText Markup Language) es el lenguaje estándar utilizado para crear y estructurar contenido en la web. HTML define la estructura básica de las páginas web mediante el uso de etiquetas (tags) que organizan el contenido en elementos como encabezados, párrafos, enlaces, imágenes, tablas y más.

Cada etiqueta de HTML se encuentra entre corchetes angulares < >, y algunas etiquetas tienen una etiqueta de cierre, lo que significa que el contenido dentro de ellas está delimitado por una apertura y un cierre. Por ejemplo:

```html
<h1>Este es un encabezado</h1>
<p>Este es un párrafo de texto.</p>
<a href="https://www.ejemplo.com">Este es un enlace</a>
```

En este ejemplo:

    <h1> es un encabezado de nivel 1 (el más importante).
    <p> crea un párrafo.
    <a> define un enlace con el atributo href que especifica la URL a la que apunta.

HTML es la base para el contenido de las páginas web, mientras que otros lenguajes como CSS (para el diseño) y JavaScript (para la interacción) se utilizan junto con HTML para mejorar la presentación y funcionalidad de las páginas.

# CSS

CSS (Cascading Style Sheets, o Hojas de Estilo en Cascada) es un lenguaje utilizado para describir el aspecto visual y el diseño de una página web. Mientras que HTML se encarga de la estructura del contenido, CSS se encarga de cómo ese contenido se ve y se presenta, permitiendo personalizar elementos como colores, fuentes, márgenes, tamaños, espaciado, distribución, y más.

CSS funciona mediante reglas que definen el estilo de uno o más elementos HTML. Cada regla consta de un selector y una serie de declaraciones que contienen propiedades y valores. Por ejemplo:

```css
/* Este es un comentario */
h1 {
  color: blue;
  font-size: 24px;
}

p {
  color: gray;
  line-height: 1.5;
}
```
En este ejemplo:

El selector h1 aplica estilos a todos los elementos  en la página.

color: blue; cambia el color del texto a azul.
font-size: 24px; define el tamaño de la fuente como 24 píxeles.

El selector p aplica estilos a los elementos:

color: gray; cambia el color del texto a gris.
line-height: 1.5; ajusta el espaciado entre las líneas del párrafo.

"Cascading" (en cascada) se refiere a cómo las reglas se aplican de manera jerárquica. Si hay varias reglas que se aplican a un mismo elemento, CSS sigue un orden de precedencia para determinar cuál se aplica. Esto se basa en la especificidad de los selectores, el orden en que aparecen las reglas y la herencia de estilos entre elementos.

CSS se puede aplicar a una página de varias maneras:

Estilos en línea: dentro de las etiquetas HTML usando el atributo style:
    
```html
<h1 style="color: red;">Este es un encabezado rojo</h1>
```

Estilos internos: dentro de una etiqueta *style* de tipo en el archivo HTML:


```html
<style>
  h1 {
    color: red;
  }
</style>
```
Estilos externos: en un archivo .css separado, vinculado al HTML con una etiqueta 

```html
<link rel="stylesheet" href="estilos.css">
```

CSS permite separar la presentación del contenido, facilitando cambios en el diseño sin tener que modificar la estructura HTML. Esto mejora la mantenibilidad y la flexibilidad de las páginas web.

# *Document Object Model* (DOM)

El DOM (Document Object Model, o Modelo de Objetos del Documento) es una representación estructurada de un documento HTML o XML que permite a los lenguajes de programación, como JavaScript, interactuar con su contenido de manera dinámica. Básicamente, convierte la página web en un conjunto de objetos accesibles y manipulables por código, permitiendo modificar el contenido, la estructura y el estilo de la página sin necesidad de recargarla.
¿Cómo funciona el DOM?

El DOM organiza los elementos del documento en una estructura jerárquica similar a un árbol, donde cada nodo representa una parte del documento, como un elemento HTML, un atributo, un texto, o un comentario. Por ejemplo, para una página HTML simple:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Mi página web</title>
  </head>
  <body>
    <h1>Bienvenido</h1>
    <p>Este es un párrafo de ejemplo.</p>
  </body>
</html>
```
El DOM se vería de manera jerárquica, como un árbol de nodos:

    html
        head
            title
                "Mi página web" (texto)
        body
            h1
                "Bienvenido" (texto)
            p
                "Este es un párrafo de ejemplo." (texto)

Tipos de nodos en el DOM:

   - Nodos de elemento: Representan las etiquetas HTML (como ```<h1>, <p>, <div>```).
   - Nodos de atributo: Representan los atributos de las etiquetas HTML (como id, class, src).
   - Nodos de texto: Contienen el contenido textual dentro de un elemento (como "Bienvenido" en el ejemplo anterior).
   - Nodos de comentario: Representan los comentarios dentro del código HTML.

# Javascript

JavaScript es un lenguaje de programación que se utiliza principalmente para agregar interactividad y dinamismo a las páginas web. A diferencia de HTML y CSS, que se encargan de la estructura y el estilo, JavaScript permite que los sitios web sean interactivos y respondan a acciones del usuario, como hacer clic en botones, enviar formularios, realizar animaciones, cargar datos sin recargar la página (mediante AJAX), entre otras muchas funcionalidades.
Características clave de JavaScript:

Lenguaje del lado del cliente: Aunque JavaScript también puede ejecutarse en el servidor (con tecnologías como Node.js), su uso principal es en el navegador web del cliente, interactuando con el DOM (Document Object Model), que representa la estructura de la página web en HTML.

Interactividad: JavaScript permite crear elementos interactivos, como menús desplegables, formularios que validan datos antes de ser enviados, y contenido dinámico que cambia sin necesidad de recargar toda la página.

Lenguaje interpretado: JavaScript no necesita ser compilado; el navegador lo interpreta directamente cuando carga la página. Esto permite realizar cambios y ver los resultados de manera inmediata.

Compatible con todos los navegadores: JavaScript es compatible con todos los navegadores web modernos, lo que lo hace extremadamente accesible para desarrolladores y usuarios.

Lenguaje basado en eventos: JavaScript responde a eventos del usuario (clics, desplazamiento, entrada de texto), del sistema (carga de la página, errores), o de elementos específicos del documento HTML.

Ejemplo básico de JavaScript:

```html
<!DOCTYPE html>
<html>
<head>
  <title>Ejemplo de JavaScript</title>
  <script>
    function mostrarMensaje() {
      alert('¡Hola, bienvenido a mi página!');
    }
  </script>
</head>
<body>
  <h1>Bienvenido</h1>
  <button onclick="mostrarMensaje()">Haz clic aquí</button>
</body>
</html>
```

En este ejemplo:

El código JavaScript está dentro de la etiqueta *script*.
La función mostrarMensaje() genera una alerta en la página cuando se ejecuta.
El botón en HTML tiene el atributo onclick, que ejecuta la función JavaScript cuando se hace clic en el botón.

## ¿Qué puede hacer JavaScript?

Manipular el DOM: JavaScript puede modificar el contenido y la estructura del documento HTML, permitiendo, por ejemplo, añadir o eliminar elementos de la página, cambiar el texto o modificar el estilo de los elementos dinámicamente.

```JavaScript
document.getElementById('miElemento').innerHTML = "Nuevo contenido";
```

 - Validar formularios: Antes de que los datos se envíen al servidor, JavaScript puede verificar si se han llenado correctamente.

```JavaScript
if (document.getElementById('nombre').value === '') {
  alert('Por favor, ingresa tu nombre');
}
```
 - Trabajar con APIs y AJAX: JavaScript permite hacer solicitudes HTTP a servidores, lo que permite cargar datos en segundo plano sin recargar toda la página.

```JavaScript
fetch('https://api.example.com/data')
  .then(response => response.json())
  .then(data => console.log(data));
```

   - Crear animaciones: Puede mover, cambiar de tamaño o hacer transiciones entre los elementos de la página, logrando animaciones suaves sin usar Flash.

   - Programación orientada a objetos y funcional: JavaScript soporta múltiples paradigmas de programación, permitiendo a los desarrolladores estructurar su código de diferentes maneras según las necesidades.

Frameworks y librerías populares:

JavaScript ha evolucionado mucho, y existen muchas librerías y frameworks que facilitan su uso:

  - jQuery: Una librería que simplifica la manipulación del DOM y las interacciones con el servidor.
  - React, Angular, Vue.js: Frameworks que facilitan la creación de interfaces de usuario dinámicas y aplicaciones web más complejas.
  - Node.js: Un entorno para ejecutar JavaScript del lado del servidor, permitiendo crear aplicaciones backend.

En resumen, JavaScript es esencial para crear sitios web modernos e interactivos, complementando a HTML y CSS para ofrecer experiencias web mucho más ricas y dinámicas.