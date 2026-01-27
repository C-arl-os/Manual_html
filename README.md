# 📘 Manual Personal de HTML  
_Apuntes diarios y ejemplos prácticos_

---

## 📌 Información general

| Campo | Detalle |
|------|--------|
| Autor | Carlos Sancir |
| Fecha inicio | 8/1/2026 |
| Objetivo | Aprender HTML desde cero |
| Nivel | Básico → Avanzado |

---

## 🧭 Índice

- [📘 Manual Personal de HTML](#-manual-personal-de-html)
  - [📌 Información general](#-información-general)
  - [🧭 Índice](#-índice)
    - [📝 Formato Markdown útil:](#-formato-markdown-útil)
  - [1️⃣ Introducción](#1️⃣-introducción)
    - [¿Qué es un elemento HTML?](#qué-es-un-elemento-html)
    - [¿Para qué sirve?](#para-qué-sirve)
  - [2️⃣ Conceptos básicos](#2️⃣-conceptos-básicos)
    - [¿Qué es una etiqueta?](#qué-es-una-etiqueta)
    - [Tipos de etiquetas](#tipos-de-etiquetas)
  - [3️⃣ Estructura básica de un documento HTML](#3️⃣-estructura-básica-de-un-documento-html)
    - [Plantilla base](#plantilla-base)
      - [Elementos sin etiqueta de cierre (Void Elements)](#elementos-sin-etiqueta-de-cierre-void-elements)
  - [4 ¿Qué son los atributos en HTML y cómo funcionan?](#4-qué-son-los-atributos-en-html-y-cómo-funcionan)
    - [Formulario de los atributos más comunes](#formulario-de-los-atributos-más-comunes)
  - [5 El elemento  en HTML](#5-el-elemento--en-html)
    - [¿Qué significa ./styles.css?](#qué-significa-stylescss)
    - [Uso del  con Google Fonts](#uso-del--con-google-fonts)
    - [Uso del  para favicon](#uso-del--para-favicon)
    - [Diferentes sintaxis más comunes.](#diferentes-sintaxis-más-comunes)
      - [Absolute URLs vs. Relative URLs](#absolute-urls-vs-relative-urls)
      - [HTML LINKS - usando imagenes](#html-links---usando-imagenes)
      - [Link para una dirección de correo](#link-para-una-dirección-de-correo)
      - [Bottones con link](#bottones-con-link)
      - [Link en titulos](#link-en-titulos)
  - [6 ¿Qué es un HTML Boilerplate??](#6-qué-es-un-html-boilerplate)
      - [Ejemplo de Boilerplate](#ejemplo-de-boilerplate)
  - [7 HTML Fundamentos](#7-html-fundamentos)
    - [1. ¿Qué significado semántico tiene un elemento div?](#1-qué-significado-semántico-tiene-un-elemento-div)
    - [2. ¿Cuándo es más apropiado usar un elemento div en HTML?](#2-cuándo-es-más-apropiado-usar-un-elemento-div-en-html)
    - [IDs y 🏷️ Classes en HTML](#ids-y-️-classes-en-html)
      - [¿Qué es una class?](#qué-es-una-class)
      - [Varias clases en un solo elementos](#varias-clases-en-un-solo-elementos)
    - [¿Qué son las HTML Entities (entidades HTML)?](#qué-son-las-html-entities-entidades-html)
    - [`¿Para qué sirve el elemento <script> en HTML?`](#para-qué-sirve-el-elemento-script-en-html)
  - [Entiende como HTML afecta SEO](#entiende-como-html-afecta-seo)
    - [¿Qué es SEP?](#qué-es-sep)
    - [¿Qué son las Open Graph Tags (OG)?](#qué-son-las-open-graph-tags-og)
    - [Open Graph más importantes](#open-graph-más-importantes)
      - [og:title](#ogtitle)
      - [og:type](#ogtype)
      - [og:image](#ogimage)
      - [og:url](#ogurl)
  - [Trabaja con elementos de Audio y Video](#trabaja-con-elementos-de-audio-y-video)
    - [¿Cúal es el Rol de las etiquetas Audio y Video, ¿Cómo puedes trabjar con ellas?](#cúal-es-el-rol-de-las-etiquetas-audio-y-video-cómo-puedes-trabjar-con-ellas)
      - [`<audi>`](#audi)
    - [Compatibilidad con varios formatos](#compatibilidad-con-varios-formatos)
    - [Elemento `<video>`](#elemento-video)
      - [Mostrar una imagen mientras carga el video](#mostrar-una-imagen-mientras-carga-el-video)

### 📝 Formato Markdown útil:
- **Negrita**
- *Itálica*
- ***Negrita e itálica***
- ~~Texto tachado~~  

---

## 1️⃣ Introducción
HTML es un lenguaje de marcado o etiquetas. Sus siglas significan **HyperText Markup Language** (Lenguaje de Marcado de Hipertexto). Sirve para crear páginas web y es el esqueleto o la estructura principal de toda página web.
### ¿Qué es un elemento HTML?
Un elemento HTML está compuesto por tres partes:

1. **Etiqueta de apertura**: Marca el inicio del elemento (ej. `<p>`)
2. **Contenido**: El texto o elementos que van dentro
3. **Etiqueta de cierre**: Marca el final del elemento (ej. `</p>`)



**Ejemplo de un elemento HTML:**

```html
<p>Hola mundo</p>
```


### ¿Para qué sirve?
- Crear la estructura de páginas web
- Organizar contenido (texto, imágenes, videos)
- Definir la semántica del contenido
- Base para aplicar estilos CSS y funcionalidad JavaScript 

---

## 2️⃣ Conceptos básicos

### ¿Qué es una etiqueta?
> Una etiqueta es una instrucción que le dice al navegador cómo mostrar el contenido. Se escribe entre corchetes angulares `< >` y puede tener atributos que modifican su comportamiento.

### Tipos de etiquetas

| Tipo | Descripción | Ejemplo |
|----|------------|--------|
| Apertura | Inicia un elemento | `<p>`, `<div>`, `<h1>` |
| Cierre | Finaliza un elemento | `</p>`, `</div>`, `</h1>` |
| Vacía (Autocerrada) | No necesita cierre | `<img>`, `<br>`, `<hr>`, `<input>` |

---

## 3️⃣ Estructura básica de un documento HTML

### Plantilla base

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Título</title>
</head>
<body>

</body>
</html>
```
#### Elementos sin etiqueta de cierre (Void Elements)
No tiene contenido
No tienen etiqueta de cierre 

**Ejemplo de un elemento HTML:**

```html
<img />
<img>
```
Ambas formas son válidas.

##  4 ¿Qué son los atributos en HTML y cómo funcionan?
Es un valor que se coloca dentro de la etiqueta de apertura de un elemnto de HTML.
- 📄 Dar información adicional.
- 📘 Definir cómo se comporta un elemento

**Sintaxis básica de un atributo**
```html
<elemento atributo="valor"></elemento>
```
👉 = Signo de asignación 
👉 valor (valor del atributo)

**Ejemplo con enlaces **
```html
<a href="https://www.freecodecamp.org/news/" target="_blank">
  Visit freeCodeCamp
</a>
```
👉href → indica la URL del enlace
👉target="_blank" → abre el enlace en una nueva pestaña

**Atributos comunes en imágenes (<img>)**
```html
<img src="cats.jpg" alt="Two tabby kittens sleeping together" />
```
- **`src`** (obligatoria): ruta de la imagen
- **`alt`** (recomendado): texto alternativo

**Atributo booleanos comunes**
| Atributo | Función |
|------|--------|
| checked | Marca de checkbox |
| disabled | Desactiva un elemento |
|readonly | Solo lectura |
| required | Campo obligatorio |
**Ejemplo con disabled**
```html
<input type="text" disabled>
```
✔ El usuario no puede escribir
❌ Si quitamos disabled, el campo se habilita

### Formulario de los atributos más comunes
| Atributo | Función |
|------|--------|
| href | ``<a>`` especifica la URL de la pagina   |
| src | ```<img>``` especifica el path o la ruta de la imagen |
|width and height | ```<img>``` provee la información para dimensionar la imagen|
| alt |  ```<img>``` provee una alternativa cuando la imagen no carga|
|style|atributo is usado para añadir color, fondo, tamaño y más|
|lang|atributo de ```<html>``` declara el lenguage de la web page|

##  5 El elemento <link> en HTML
El elemento ```<link>``` se usa para utilizar recursos externo de la paginas como:
1. Hojas de estilo CSS
2. Fuentes externas
3. íconos de sitios externos
   
**Sintaxis básica para CSS externo**
```html
<link rel="stylesheet" href="./styles.css" />

```
***Atributos importantes:***
- rel → define la relación entre el recurso y el documento HTML
- href → indica la ubicación del archivo externo

### ¿Qué significa ./styles.css?
1. ./ indica que el archivo esta en la misma carpeta.
2. styles.css es archivo de CSS
   
```html
<head>
  <link rel="stylesheet" href="./styles.css" />
</head>


```
### Uso del <link> con Google Fonts
```html
<link rel="preconnect" href="https://fonts.googleapis.com" />
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
<link
  href="https://fonts.googleapis.com/css2?family=Playwrite+CU:wght@100..400&display=swap"
  rel="stylesheet"
/>

```
**¿Para qué sirve rel="preconnect"?**
- Hace que el navegador se conecte antes al servidor
- Mejora el rendimiento y velocidad de carga

### Uso del <link> para favicon
```html
<link rel="icon" href="favicon.ico" />
```
- Un ícono pequeño
- Aparece en la pestaña del navegador
- Representa la marca o sitio web

### Diferentes sintaxis más comunes.
**1 ```<a>``` definiendo un link**
```html
<a href="url">link text</a>
```

***HTML links - Atributos***
| Atributo | Función |
|------|--------|
| _self | Abre en la misma ventana |
| _blank | Abre el documento en una nueva ventana |
|_parent| Abre la ventana en el parent frame |
| _top | abre el documento en todo el cuerpo de la pagina|

#### Absolute URLs vs. Relative URLs
```html
<h2>Absolute URLs</h2>
<p><a href="https://www.w3.org/">W3C</a></p>
<p><a href="https://www.google.com/">Google</a></p>

<h2>Relative URLs</h2>
<p><a href="html_images.asp">HTML Images</a></p>
<p><a href="/css/default.asp">CSS Tutorial</a></p>
```

#### HTML LINKS - usando imagenes
```html
<a href="default.asp">
<img src="smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;">
</a>
```

#### Link para una dirección de correo
```html
<a href="mailto:someone@example.com">Send email</a>
```
#### Bottones con link
```html
<button onclick="document.location='default.asp'">HTML Tutorial</button>
```
#### Link en titulos
```html
<a href="https://www.w3schools.com/html/" title="Go to W3Schools HTML section">Visit our HTML Tutorial</a>
```

##  6 ¿Qué es un HTML Boilerplate??
Son los siemntos o la estructura de tu pagina web es donde se inicia todo y contendra
todo el contenido que deseas a;adir dentro de el, ademas de asegurar la compatibilidad con
navegadores.


#### Ejemplo de Boilerplate
```htm
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>freeCodeCamp</title>
    <link rel="stylesheet" href="./styles.css" />
  </head>
  <body>
  </body>
</html>

```
**`<!DOCTYPE html>`**
Le dice al navegador que esta pagina se realizo
cob HTML5.

**`<html lang="en">`**
Es la encargada de contener todo el contenido
de la pagina web ademas de indicar el idioma que esta esta
es importante para
- Accesibilidad

- SEO

- Lectores de pantalla

**`<head>`**

Es la información que no se ve reflejada visualmente
en lapagina pero es la encargada de configurar con componentes externos
a la pagina como:
- Codificacion de caracteres
- Ajuste para moviles
- Titulo de pestaña
- Enlaces a CSS
- ETC
  
**`<meta charset="UTF-8" />`**
Este es un estandar de codificacion que se usa
en la escritura de la pagina web y caracteres.
- Permite usar:
- Tildes (á, é, í)
- Ñ
- Símbolos especiales

**`<meta name="viewport" content="width=device-width, initial-scale=1.0" />`**

Hace que la pagina se ajuste a diferentes tipo
de pantallas como:
- Celulares
- Tablets
- Pantallas pequeñas

**`<link rel="stylesheet" href="./styles.css" />`**
Conecta el archivo con estilos CSS externo a HTML.

**`<body> `**
Aqui va todo lo que puede ser visible.
como:
- Títulos
- Párrafos
- Imágenes
- Botones
- Formularios


## 7 HTML Fundamentos

### 1. ¿Qué significado semántico tiene un elemento div?
El elemento `<div>` no tiene un significado semantico.

Es un contenedor generico ya que no describe expecificamente
que tipo de contenido contendra adentro o no se puede tener informacion
adicional sobre su proposito.

### 2. ¿Cuándo es más apropiado usar un elemento div en HTML?

Cuando se agrupa contenido relacionado para aplicar estilos (CSS).

📌 Explicación:
El `<div> ` se usa principalmente para:
- Agrupar elementos
- Aplicar estilos CSS
- Manipular contenido con JavaScript

No se debe usar para dar estructura semántica a la página.

***HTML links - Atributos***
| Atributo | Función | Uso Principal
|------|--------|--------|
| div | NO | Agrupar contenido para estilos |
| section | SI | Dividir el contenido en seccion|
| article | SI | Contenido independiente|
| nav| SI| Navegación|
|  footer  |   SI  |  Pie de página   |


### IDs y 🏷️ Classes en HTML

Un id es un identificador único una vez se coloque dentro de la página.


***Ejemplo**
```HTML
<h1 id="title">Movie Review Page</h1>


```
1. Aplicar estilos CSS.
2. Manipular el elemento con JavaScript

**Usar un id en CSS**
```CSS
#title {
  color: red;
}


```
El simbolo `#` Significa que se va a seleccioanr un id

Reglas Importantes:
- Deben ser únicos
- No puede tener espacios
- solor usar
  - Letras
  - Números
  - Guiones
  - Guiones bajos
  
Si usas un Id dos veces puede fallar CSS o JS
puede seleccionar un elemento incorrecto


#### ¿Qué es una class?

Sirve para agrupar varios elementos que compartiran un mismo estilo
o un mismo comportamiento, Este se puede repetir varis veces.

```HTML
<div class="box"></div>


```
```CSS
.box {
  width: 100px;
  height: 100px;
}

```
Todos los elementos class="box" tendran el mismo tamaño

#### Varias clases en un solo elementos
Un elemento puede tener más de una clase, sepadas por espacio
```HTML
<div class="box red-box"></div>


```
```CSS
.red-box {
  background-color: red;
}


```
- box -> tamaño
- red-box -> color

Puede tener varios elementos
```HTML
<div class="box red-box"></div>
<div class="box blue-box"></div>
<div class="box red-box"></div>
<div class="box blue-box"></div>


```

| Atributo | Función | |
|------|--------|-------- |
| ¿Único? |SI |NO |
| ¿Se puede repetir? | NO | SI|
|¿Puede tener espacios?| NO | SI|
| Selector CSS | #ID | .CLASS |

### ¿Qué son las HTML Entities (entidades HTML)?
Una entidad HTML es un caracter referenciado o una forma
especial de escribir ciertos caracteres que esta reservador por el propio
lenguaje, para que el navegador los interprete como texxto y no como
código HTML.

Existen debido a que algunos caracteres tienen significado ejemplo
`<>`
| Result | Description               | Name     | Number   |
|--------|---------------------------|----------|----------|
|        | non-breaking space        | `&nbsp; `  | `&#160; `  |
| <      | less than                 | `&lt; `    | `&#60;`    |
| >      | greater than              | `&gt; `    | `&#62; `   |
| &      | ampersand                 | `&amp; `   |` &#38;`    |
| "      | double quotation mark     | `&quot; `  | `&#34;`    |
| '      | single quotation mark     | `&apos; `  | `&#39; `   |
| ¢      | cent                      | `&cent; `  | `&#162;`   |
| £      | pound                     | `&pound;`  | `&#163; `  |
| ¥      | yen                       | `&yen;`    | `&#165; `  |
| €      | euro                      | `&euro;`   | `&#8364;`  |
| ©      | copyright                 | `&copy; `  | `&#169; `  |
| ®      | registered trademark      | `&reg;`    | `&#174;`   |


```HTML
<!DOCTYPE html>
<html>
<body>

<h1>HTML Entity Example</h1>

<h2>The yen sign: &yen;</h2>

</body>
</html>


```

### `¿Para qué sirve el elemento <script> en HTML?`

Se ua para ejecutar codigo  que normalmente es JavaScript, detron de la pagina web

Permite:

- Interactividad

- Formularios dinámicos

- Validaciones en tiempo real

- Juegos

- Animaciones

- Botones que reaccionan

```HTML
<body>
  <script>
    alert("Welcome to freeCodeCamp");
  </script>
</body>

```
Mala practica, para proyectos grandes.

Buena practica

```HTML
<script src="path-to-javascript-file.js"></script>


```
## Entiende como HTML afecta SEO

### ¿Qué es SEP?
significa Search Engine Optimization, Son un conjunto de 
practicas que ayuda a optimizar los motores de busquedas de las 
paginas web, que aprecen en Google, Brave, Bing, etc
- Aparezca en Google, Bing, etc.
- Se muestra más arroba en los resultados.
- Reciba más visitas

**¿Qué es la meta descripción?**
Es una breve descripción del contenido que tiene la pagina web
se define el elemento `<meat>`  dentro del `<head>` del HTML.

Ejmplo

```HTML
<meta
  name="description"
  content="Discover expert tips and techniques for gardening in small spaces."
/>

```

***¿Qué hace cada parte?***
1. meta -> elemento especial para metadatos.
2. name="description" -> indica que es una descripción.
3. content="..." -> el texto que describe la página.

***¿Donde aparece la descripción?***

En los resultados del buscador, debajo del enlace del sitio.

***¿Afecta el posicionamiento?***
- No afecta directamente al ranking.
- Sí puede aumentar los clics
  - Explica claramente de que trata el contenido dentro de la pagína.
  - Hace que más personas quieran entrar.

### ¿Qué son las Open Graph Tags (OG)?

Son meta etiquetas que controlan cómo se ve tu pagína cuando alguien 
la comparte en redes sociales como:
1. Facebook
2. Linkdln
3. WhatsApp
   
No cambian cómo se ve tu pagína, solo cómo al compartir el link.

***¿Para qué sirve?***
- Mostrar un titulo atractivo.
- Una imagen bonita.
- Una descripción clara
- Hacer que las personas hagan mas click

***¿Dónde se escriben?***
Dentro del `<head>` del Html usando `<meta>`

```HTML
<meta property="og:title" content="freeCodeCamp.org" />

```

### Open Graph más importantes

#### og:title

Define el título que aparece en redes sociales al comparti el link.

```HTML
<meta property="og:title" content="freeCodeCamp.org" />

```

#### og:type
Indica qué tipo de contenido es:
1. website
2. article
3. video
4. music

```HTML
<meta property="og:type" content="website" />

```

#### og:image

Es la imagen que muestra en la publicación.

Recomendado.
- 1200 x 630 px
- Buena calidad
- Relación correcta

```HTML
<meta property="og:image" content="https://example.com/image.png" />

```

#### og:url

Es la URL ofical del contenido compartido
```HTML
<meta property="og:url" content="https://www.freecodecamp.org" />

```
## Trabaja con elementos de Audio y Video

### ¿Cúal es el Rol de las etiquetas Audio y Video, ¿Cómo puedes trabjar con ellas?

#### `<audi>`
El elemenot `<audio>` sirve para agregar sonido a una página web (música,efetos,grabaciones,etc)

**Ejemplo**
```HTML
<audio src="audio.mp3"></audio>
```

**Mostrar el reproductor (play, pauso,volumen)**
Para que el usuario pueda controlar el audio, con los controles basicos se usa el atributo 
controls
```HTML
<audio src="audio.mp3" controls></audio>
```
**Repetir el audio automáticamente Y silenciar el audio**
El atributo loop hace que el audio se repita cuando termina:
```HTML
<audio src="audio.mp3" controls loop></audio>
<audio src="audio.mp3" controls muted></audio>

```

### Compatibilidad con varios formatos
No todos los navegadores tienen la capacidad de soportar
algunos formatos. Por eso se usa la etiqueta `<source>`

```HTML
<audio controls>
  <source src="audio.ogg" type="audio/ogg">
  <source src="audio.wav" type="audio/wav">
  <source src="audio.mp3" type="audio/mpeg">
</audio>

<video controls width="400">
  <source src="video.mp4" type="video/mp4">
  <source src="video.webm" type="video/webm">
  Tu navegador no soporta video.
</video>

```
### Elemento `<video>`
El elemento `<video> `sirve para mostrar videos en una página web.

```HTML
<video src="video.mp4" controls></video>

```
**Atributos comunes de `<video>`
**
Estos funcionan igual que en `<audio>`:

- controls	Muestra play, pausa, volumen
- loop	Repite el video
- muted	Inicia en silencio
- autoplay	Reproduce automáticamente
- width	Cambia el tamaño

#### Mostrar una imagen mientras carga el video
El atributo poster muestra una imagen antes de que el video empiece:
```HTML
<video
  src="video.mp4"
  controls
  poster="imagen.jpg"
  width="400">
</video>
```
| Elemento / Atributo | Función | Aplica a |
|--------------------|--------|----------|
| `<audio>` | Agrega sonido a una página web | Audio |
| `<video>` | Agrega video a una página web | Video |
| `src` | Ruta del archivo de audio o video | Audio / Video |
| `controls` | Muestra controles (play, pausa, volumen) | Audio / Video |
| `loop` | Reproduce el contenido en bucle | Audio / Video |
| `muted` | Inicia el audio o video silenciado | Audio / Video |
| `autoplay` | Reproduce automáticamente al cargar la página | Audio / Video |
| `poster` | Muestra una imagen mientras el video carga | Solo Video |
| `width` | Define el ancho del video | Solo Video |
| `<source>` | Permite usar varios formatos compatibles | Audio / Video |
