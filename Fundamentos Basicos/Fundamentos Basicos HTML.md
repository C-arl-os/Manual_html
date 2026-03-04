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
  - [Trabajar con Imagenes y SVGs](#trabajar-con-imagenes-y-svgs)
    - [Optimización de Activos Multimedia en la Web (Imágenes)](#optimización-de-activos-multimedia-en-la-web-imágenes)
    - [¿Cuáles son los diferentes tipos de licencias de imagen y cómo funcionan?](#cuáles-son-los-diferentes-tipos-de-licencias-de-imagen-y-cómo-funcionan)
      - [1. Copyright y “All Rights Reserved”](#1-copyright-y-all-rights-reserved)
      - [2. Fair Use (Uso legítimo)](#2-fair-use-uso-legítimo)
      - [3. Licencias permisivas (Permissive Licenses)](#3-licencias-permisivas-permissive-licenses)
      - [4. Public Domain (Dominio Público)](#4-public-domain-dominio-público)
      - [5. Búsqueda de imágenes por licencia](#5-búsqueda-de-imágenes-por-licencia)
      - [6. Buenas prácticas profesionales](#6-buenas-prácticas-profesionales)
    - [¿Qué son los SVG y cuándo debes usarlos?](#qué-son-los-svg-y-cuándo-debes-usarlos)
    - [Desventaja principal de las imágenes raster](#desventaja-principal-de-las-imágenes-raster)
      - [2. ¿Qué es un SVG?](#2-qué-es-un-svg)
      - [Ventaja principal de los SVG](#ventaja-principal-de-los-svg)
    - [SVG embebido directamente en HTML](#svg-embebido-directamente-en-html)
  - [Trabaja con el iframe Element](#trabaja-con-el-iframe-element)
      - [Elementos Reemplazados en HTML y CSS](#elementos-reemplazados-en-html-y-css)
  - [¿Comó trabajar con los Links?](#comó-trabajar-con-los-links)
    - [¿Cuáles son los diferentes tipos de atributos de destino y cómo funcionan?](#cuáles-son-los-diferentes-tipos-de-atributos-de-destino-y-cómo-funcionan)
      - [Atributo `target` en HTML](#atributo-target-en-html)
    - [Tipos de `target` que debes saber](#tipos-de-target-que-debes-saber)
      - [1️⃣ `_self`(por defecto)](#1️⃣-_selfpor-defecto)
      - [2️⃣ \_blank](#2️⃣-_blank)
      - [3️⃣ \_parent](#3️⃣-_parent)
      - [4️⃣ \_top](#4️⃣-_top)
      - [5️⃣ \_unfencedTop (⚗️ experimental)](#5️⃣-_unfencedtop-️-experimental)
    - [¿Cúal es la diferencia entre  Absolute y Relative Paths?](#cúal-es-la-diferencia-entre--absolute-y-relative-paths)
      - [🌐 Absolute Path (Ruta absoluta)](#-absolute-path-ruta-absoluta)
    - [¿Cuál es la diferencia entre barras, un punto simple y un punto doble en la sintaxis de ruta?](#cuál-es-la-diferencia-entre-barras-un-punto-simple-y-un-punto-doble-en-la-sintaxis-de-ruta)
      - [1️⃣ Slash / (separador de rutas)](#1️⃣-slash--separador-de-rutas)
      - [2️⃣ Single Dot . (directorio actual)](#2️⃣-single-dot--directorio-actual)
      - [3️⃣ Double Dot .. (directorio padre)](#3️⃣-double-dot--directorio-padre)
    - [¿Qué son los Link States y por qué importan?](#qué-son-los-link-states-y-por-qué-importan)
      - [1️⃣ :link (estado por defecto)](#1️⃣-link-estado-por-defecto)
      - [2️⃣ :visited](#2️⃣-visited)
      - [3️⃣ :hover](#3️⃣-hover)
      - [4️⃣ :focus](#4️⃣-focus)
      - [5️⃣ :active](#5️⃣-active)

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


## Trabajar con Imagenes y SVGs

### Optimización de Activos Multimedia en la Web (Imágenes)
La optimización de imágenes es una práctica fundamental en el desarrollo web moderno, ya que impacta directamente en:

Performance

- Tiempo de carga
- Consumo de ancho de banda
- Experiencia de usuario (UX)
- SEO
  
Existen tres ejes técnicos principales para la optimización de imágenes:

1. Dimensiones (size / resolution)
2. Formato del archivo (file format)
3. Compresión (compression)
1. Dimensiones de la imagen (Image Size / Resolution)
Definición técnica

Las dimensiones de una imagen corresponden a su ancho y alto en píxeles, y deben coincidir con el tamaño final de renderizado definido por CSS o el layout del navegador.

Servir imágenes con dimensiones superiores al tamaño renderizado implica transferencia innecesaria de datos.

Ejemplo técnico

```CSS

img.hero {
  width: 640px;
  height: 480px;
}
```

Imagen servida	Imagen renderizada	Impacto
1920×1080	640×480	❌ Descarga excesiva
640×480	640×480	✅ Óptimo


Aunque el navegador renderiza ambas imágenes al mismo tamaño visual, el archivo completo se descarga antes del escalado, lo cual incrementa:

Tiempo de carga

Uso de datos móviles

Costo de transferencia

| Formato | Tipo de compresión | Transparencia | Uso recomendado |
|-------|--------------------|--------------|----------------|
| JPG   | Con pérdida (lossy) | ❌ No        | Fotografías (con cuidado) |
| PNG   | Sin pérdida        | ✅ Sí        | Gráficos, íconos |
| WEBP  | Con / sin pérdida  | ✅ Sí        | Web moderna |
| AVIF  | Con / sin pérdida  | ✅ Sí        | Máxima optimización |
Consideraciones modernas

PNG y JPG son formatos tradicionales

WEBP y AVIF ofrecen:

  - Menor tamaño de archivo
  - Mejor relación calidad/peso
  - Optimización para HTTP/2 y HTTP/3


|Tipo|	Descripción|
|---------|--------------------------|
|Lossless|	No se pierde información; el archivo original puede reconstruirse|
|Lossy|	Se descarta información para reducir tamaño|

### ¿Cuáles son los diferentes tipos de licencias de imagen y cómo funcionan?

Las imágenes digitales son consideradas propiedad intelectual (intellectual property), lo que implica que están protegidas por leyes de derechos de autor (copyright) desde el momento de su creación.

Por defecto, toda imagen tiene copyright, incluso si se encuentra públicamente en internet.

#### 1. Copyright y “All Rights Reserved”
Definición técnica

Cuando una imagen está bajo All Rights Reserved, el autor o editor conserva todos los derechos legales sobre ella.

Esto significa que no puedes usar la imagen libremente en un sitio web, aplicación o proyecto sin autorización expresa.

Opciones legales para usar una imagen con copyright

Solo puedes usar este tipo de imagen si cumples al menos una de las siguientes condiciones:
- Permiso escrito del autor
- Compra de una licencia
- Uso legítimo bajo fair use

#### 2. Fair Use (Uso legítimo)
Definición técnica

Fair use es una excepción legal que permite el uso limitado de material protegido sin permiso del autor, siempre que el uso sea:

Limitado

Transformativo

¿Qué significa transformativo?

El contenido original debe cambiar su propósito, no solo reutilizarse.

Ejemplos válidos de fair use
- Crítica o reseña de una obra artística
- Comentario educativo
- Parodia
- Análisis académico

Ejemplos NO válidos

- Usar una imagen solo como decoración
- Copiar una imagen para un blog sin modificarla
- Usar imágenes protegidas en un portafolio comercial

📌 Nota técnica importante

Fair use no es automático ni universal; depende del contexto legal y jurisdicción.

#### 3. Licencias permisivas (Permissive Licenses)

Algunos autores publican sus imágenes bajo licencias permisivas, lo que permite su uso bajo ciertas condiciones.

Creative Commons (CC)

Creative Commons es una familia de licencias que definen cómo puede usarse una imagen.

Características generales:
- Permiten uso público
- Imponen reglas específicas
- Requieren leer la licencia antes de usar

Tabla de licencias Creative Commons (Markdown)
| Licencia | ¿Uso comercial? | ¿Modificar? | ¿Atribución? |
|--------|------------------|-------------|--------------|
| CC BY  | ✅ Sí            | ✅ Sí       | ✅ Obligatoria |
| CC BY-SA | ✅ Sí         | ✅ Sí       | ✅ + misma licencia |
| CC BY-ND | ✅ Sí         | ❌ No       | ✅ Sí |
| CC BY-NC | ❌ No         | ✅ Sí       | ✅ Sí |
| CC0    | ✅ Sí            | ✅ Sí       | ❌ No |

BSD License (ej. freeCodeCamp)

Licencia muy permisiva

Permite uso, modificación y redistribución

Usualmente asociada a proyectos open source

Puede requerir que tu proyecto también sea abierto

#### 4. Public Domain (Dominio Público)
Definición técnica

Una imagen en dominio público:

- No tiene copyright
- Puede usarse sin restricciones
- No requiere atribución
- Puede modificarse libremente
- Creative Commons Zero (CC0)

Las imágenes bajo CC0 están explícitamente cedidas al dominio público.

📌 Principio técnico

CC0 = uso libre, sin atribución, sin restricciones

#### 5. Búsqueda de imágenes por licencia
Buenas prácticas técnicas

1. Filtrar imágenes por licencia en buscadores
2. Verificar siempre la fuente original
3. Leer la licencia completa (no solo el resumen)
4. Plataformas comunes de imágenes libres
5. Pixabay
6. Unsplash
7. (Aun así, revisar condiciones específicas)

#### 6. Buenas prácticas profesionales
- Nunca asumir que una imagen es libre
- Verificar siempre la licencia
- Atribuir cuando sea requerido
- Evitar fair use en proyectos comerciales
- Preferir CC0 o licencias permisivas


### ¿Qué son los SVG y cuándo debes usarlos?


Antes de entender qué es un SVG, es necesario comprender cómo funcionan los formatos de imagen más comunes.

**Imágenes raster (PNG, JPG)**
Los formatos como **PNG** y **JPG** son imágenes **raster** (mapa de bits).

**Definición técnica:**  
Una imagen raster está compuesta por una **matriz de píxeles**, donde cada píxel almacena un valor de color específico.


---

### Desventaja principal de las imágenes raster

Las imágenes raster **no escalan correctamente**.

- Al aumentar su tamaño:
  - Los píxeles se agrandan
  - La imagen se vuelve pixelada o borrosa
- No se genera nueva información visual

**Ejemplo común:**  
Aumentar el tamaño de un PNG pequeño usando CSS provoca pérdida de nitidez.

---

#### 2. ¿Qué es un SVG?

**Definición técnica**
**SVG** significa **Scalable Vector Graphics** (Gráficos Vectoriales Escalables).

Un SVG:
- No está basado en píxeles
- Utiliza **vectores matemáticos**
- Dibuja gráficos usando puntos, líneas, curvas y rutas


---

***Desventaja principal de las imágenes raster***

Las imágenes raster **no escalan correctamente**.

- Al aumentar su tamaño:
  - Los píxeles se agrandan
  - La imagen se vuelve pixelada o borrosa
- No se genera nueva información visual

**Ejemplo común:**  
Aumentar el tamaño de un PNG pequeño usando CSS provoca pérdida de nitidez.

---


---

#### Ventaja principal de los SVG

Un SVG puede **escalarse a cualquier tamaño sin perder calidad**.

Esto lo hace ideal para:
- Diseño responsive
- Pantallas de alta resolución
- Zoom sin distorsión

---
**1. SVG como XML y HTML**

Característica técnica clave

Los SVG almacenan su información en **XML**, lo que implica que:

- Son archivos de texto
- Pueden abrirse en editores de código
- Pueden integrarse directamente en HTML

---

### SVG embebido directamente en HTML

```html
<svg width="100" height="100" viewBox="0 0 100 100"
     xmlns="http://www.w3.org/2000/svg">
  <circle cx="50" cy="50" r="45"
          stroke="black" stroke-width="4"
          fill="yellow" />
  <circle cx="35" cy="40" r="5" fill="black" />
  <circle cx="65" cy="40" r="5" fill="black" />
  <path d="M35 65 Q50 80 65 65"
        stroke="black" stroke-width="4"
        fill="transparent" />
</svg>
```
```HTML
<svg width="50" height="50" viewBox="0 0 24 24"
     fill="gold" xmlns="http://www.w3.org/2000/svg">
  <path d="M12 2L14.9 8.6L22 9.3L17 14.1L18.3 21.2
           L12 17.8L5.7 21.2L7 14.1L2 9.3L9.1 8.6L12 2Z"/>
</svg>

```

*Ejemplo Completo*
```HTML
<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Heart Icon</title>
  </head>
  <body>
    <svg width="24" height="24" viewBox="0 0 24 24" fill="red">
      <path
        d="M12 21s-6-4.35-9.33-8.22C-.5 7.39 3.24 1 8.4 4.28 10.08 5.32 12 7.5 12 7.5s1.92-2.18 3.6-3.22C20.76 1 24.5 7.39 21.33 12.78 18 16.65 12 21 12 21z"
      ></path>
    </svg>
  </body>
</html>
```

## Trabaja con el iframe Element

#### Elementos Reemplazados en HTML y CSS

 **¿Qué son los elementos reemplazados?**
Los **elementos reemplazados** son elementos HTML cuyo contenido **no es controlado por CSS ni por HTML interno**, sino que proviene de un **recurso externo** (imagen, video, otro sitio web, etc.).  
El navegador **reemplaza** el elemento por ese recurso.

---

 Características importantes
- El contenido viene de una fuente externa
- CSS **NO puede modificar el contenido interno**
- CSS **SÍ puede controlar el contenedor**
- Tienen dimensiones propias (ancho y alto naturales)
- No soportan pseudoelementos `::before` y `::after`

---

 Ejemplos comunes de elementos reemplazados

 Imagen `<img>`
```html
<img src="imagen.jpg" alt="Ejemplo de imagen">
img {
  width: 200px;
  border: 2px solid red;
}
✔ Puedes cambiar tamaño, bordes y posición
✖ No puedes cambiar la imagen con CSS

Iframe <iframe>
<iframe src="https://example.com" width="300" height="200"></iframe>
iframe {
  border: 3px solid blue;
}
✔ Puedes estilizar el marco
✖ No puedes modificar el contenido del sitio incrustado

Video <video>
<video src="video.mp4" controls width="300"></video>
video {
  filter: grayscale(100%);
}
✔ Puedes aplicar filtros visuales
✖ No puedes editar el contenido del video

Input tipo imagen <input type="image">
<input type="image" src="boton.png" alt="Enviar">
Este tipo de input se comporta como una imagen, por eso 
```

```HTML

<iframe
  title="Map of the Royal Observatory, Greenwich, London"
  width="300"
  height="200"
  src="https://www.openstreetmap.org/export/embed.html?bbox=-0.004017949104309083%2C51.47612752641776%2C0.00030577182769775396%2C51.478569861898606&amp;layer=mapnik">
</iframe>

```

## ¿Comó trabajar con los Links?

### ¿Cuáles son los diferentes tipos de atributos de destino y cómo funcionan?

#### Atributo `target` en HTML

El atributo `target` se usa en las etiquetas `<a>` para decirle al navegador dónde abrir el enlace.

```HTML
<a href="https://freecodecamp.org" target="_blank">Visit freeCodeCamp</a>

```

### Tipos de `target` que debes saber

#### 1️⃣ `_self`(por defecto)
Abre el encale en la misma pestaña.
No es obligatorio escribirlo

```HTML
<a href="page.html" target="_self">Ir a página</a>

```
Si no pones target, el navegador asume _self.

#### 2️⃣ _blank

Abre el enlace en una nueva pestaña (o ventana).

Muy usado para enlaces externos.
```HTML
<a href="https://google.com" target="_blank">Google</a>


⚠️ Buena práctica (extra):

<a href="https://google.com" target="_blank" rel="noopener noreferrer">
  Google
</a>
```
#### 3️⃣ _parent

Abre el enlace en el contenedor padre.

Se usa cuando hay iframes.
```HTML
<a href="home.html" target="_parent">Ir al sitio principal</a>
```

📝 Si no usas iframes, casi no lo necesitas.

#### 4️⃣ _top

Abre el enlace en la ventana completa del navegador.

Ignora cualquier iframe anidado.
```HTML
<a href="home.html" target="_top">Salir del iframe</a>
```

#### 5️⃣ _unfencedTop (⚗️ experimental)

Solo para APIs nuevas (FencedFrame).

No lo uses por ahora.

| Target         | ¿Dónde abre?         | ¿Cuándo usarlo?        |
|---------------|----------------------|------------------------|
| `_self`        | Misma pestaña        | Navegación normal      |
| `_blank`       | Nueva pestaña        | Enlaces externos       |
| `_parent`      | Contenedor padre     | Dentro de iframes      |
| `_top`         | Ventana completa     | Salir de iframes       |
| `_unfencedTop` | Experimental         | No necesario           |

### ¿Cúal es la diferencia entre  Absolute y Relative Paths?
Un path (ruta) es la forma de indicar dónde está un archivo (HTML, imagen, CSS, JS, etc.) dentro de un sistema de archivos o en la web.

- En desarrollo web existen dos tipos importantes:
- Absolute Path (ruta absoluta)
- Relative Path (ruta relativa)

#### 🌐 Absolute Path (Ruta absoluta)

Una ruta absoluta es la dirección completa hacia un recurso.

🔹 Características

Empieza desde la raíz

Incluye:
- Protocolo (https, http, file)
- Dominio (si es web)
- Todas las carpetas
- Nombre del archivo

```HTML
✅ Ejemplo en la web
<a href="https://design-style-guide.freecodecamp.org/img/fcc_secondary_small.svg">
  View fCC Logo
</a>

```

Partes importantes:
- Protocolo: https
- Dominio: design-style-guide.freecodecamp.org
- Archivo: fcc_secondary_small.svg

```HTML
✅ Ejemplo en computadora local
<a href="/Users/user/Desktop/fCC/pages/about.html">
  About Page
</a>
```

Y en el navegador se vería así:

file:///Users/user/Desktop/fCC/pages/about.html

📁 Relative Path (Ruta relativa)

Una ruta relativa indica la ubicación del archivo en relación al archivo actual.

🔹 Características
- ❌ No usa protocolo
- ❌ No usa dominio
- ✔️ Es más corta
- ✔️ Ideal para enlaces internos

```HTML
✅ Ejemplo (mismo folder)
<a href="about.html">About Page</a>
```
📌 Esto funciona porque:
contact.html
about.html
están en la misma carpeta

📍 Ejemplos comunes de rutas relativas
<img src="img/logo.png">        <!-- Carpeta hija -->
<img src="../img/logo.png">     <!-- Carpeta anterior -->
<link rel="stylesheet" href="css/styles.css">

📊 Tabla resumen (para apuntes)
| Tipo de Path     | ¿Qué es?                                   | ¿Cuándo usarlo? |
|------------------|--------------------------------------------|-----------------|
| Absolute Path    | Ruta completa desde la raíz o dominio      | Enlaces externos |
| Relative Path    | Ruta basada en la ubicación actual         | Enlaces internos |

### ¿Cuál es la diferencia entre barras, un punto simple y un punto doble en la sintaxis de ruta?
Slashes, . y .. en rutas (Path Syntax)

Cuando ves rutas como estas:

/public/logo.png
./script.js
../styles.css


estás viendo sintaxis de rutas de archivos.
Hay 3 elementos clave que debes conocer:

#### 1️⃣ Slash / (separador de rutas)

El slash sirve para separar carpetas y archivos.

🔹 Tipos
- / → forward slash (web, Linux, macOS) ✅
- \ → backslash (Windows) ❌ en HTML
- En HTML siempre se usa /, aunque estés en Windows.

✅ Ejemplo
<img src="public/logo.png">


Esto significa:
- carpeta public
- archivo logo.png

#### 2️⃣ Single Dot . (directorio actual)

El punto simple (.) significa: “estoy en la carpeta actual”

🔹 ¿Para qué sirve?
- Asegura que la ruta sea relativa
- Muy común en HTML, CSS y JS

✅ Ejemplo
<script src="./script.js"></script>

**El navegador busca script.js en la misma carpeta del archivo actual.**

#### 3️⃣ Double Dot .. (directorio padre)

El doble punto (..) significa:
- “sube una carpeta”

🔹 Muy usado para:
- Acceder a archivos fuera de la carpeta actual
```HTML
✅ Ejemplo
<link rel="stylesheet" href="../styles.css">
```

📌 Primero sube un nivel, luego busca styles.css.

📁 Ejemplo con estructura de carpetas
my-app/
├─ public/
│  ├─ favicon.ico
│  ├─ index.html
├─ src/
│  ├─ index.css
│  ├─ index.js

🔹 Desde public/index.html

**Cargar favicon.ico (misma carpeta):**
```HTML
<link rel="icon" href="./favicon.ico">
```


**Cargar index.css (otra carpeta):**
```HTML
<link rel="stylesheet" href="../src/index.css">
```
📊 Tabla resumen (para apuntes)
| Símbolo | Significado            | Uso común |
|-------|------------------------|-----------|
| `/`   | Separador de carpetas  | Navegar rutas |
| `.`   | Carpeta actual         | Ruta relativa |
| `..`  | Carpeta padre          | Subir niveles |

🧠 Regla mental rápida (muy importante)

1. / → entra en carpetas
2. . → aquí mismo
3. .. → sube una carpeta


### ¿Qué son los Link States y por qué importan?

Un link state es el estado visual en el que se encuentra un enlace según cómo el usuario interactúa con él.

👉 Por eso:
- A veces es azul
- Luego se vuelve morado
- Cambia al pasar el mouse
- Cambia al hacer clic
- Todo eso se controla con CSS usando pseudo-clases.

*Los 5 estados de un enlace*
#### 1️⃣ :link (estado por defecto)

Enlace no visitado

Es la base de todos los estilos
```HTML
a:link {
  color: blue;
}

```
📝 Normalmente no se escribe porque el navegador ya lo aplica.

#### 2️⃣ :visited

Se aplica cuando el usuario ya visitó el enlace
Por defecto: morado

```HTML
a:visited {
  color: brown;
}
```
✔️ Útil para:
- Documentación
- Saber qué páginas ya se leyeron

#### 3️⃣ :hover
- Se activa cuando el mouse pasa encima
- Ayuda a indicar que algo es clickeable
```HTML
a:hover {
  color: red;
}
```
Muy importante para experiencia de usuario (UX)

#### 4️⃣ :focus
Se activa cuando el enlace recibe foco
Ej: usando la tecla Tab

```HTML
a:focus {
  color: green;
}
```

♿ Importante para accesibilidad

#### 5️⃣ :active

Cuando el enlace está siendo clickeado
Dura muy poco tiempo
```HTML
a:active {
  color: black;
}
```

**Da feedback inmediato al usuario**
📊 Tabla resumen (para apuntes)
| Estado     | ¿Cuándo ocurre?                     | Uso principal |
|-----------|-------------------------------------|---------------|
| `:link`    | Enlace no visitado                  | Estilo base |
| `:visited` | Enlace ya visitado                  | Historial visual |
| `:hover`   | Mouse encima del enlace             | Interacción |
| `:focus`   | Seleccionado con teclado (Tab)      | Accesibilidad |
| `:active`  | Mientras se hace clic               | Feedback |

**Orden correcto en CSS (MUY IMPORTANTE)**
Si escribes varios estados, deben ir en este orden:

a:link
a:visited
a:hover
a:focus
a:active


📌 Truco para recordarlo:
L V H F A → Love Visits Hover Focus Active
```CSS
🧪 Ejemplo completo (simple)
a:link {
  color: blue;
}

a:visited {
  color: purple;
}

a:hover {
  color: red;
}

a:focus {
  color: green;
}

a:active {
  color: black;
}
```
