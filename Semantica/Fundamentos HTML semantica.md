# 📘 Manual Semantica en HTML
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
- [📘 Manual Semantica en HTML](#-manual-semantica-en-html)
  - [📌 Información general](#-información-general)
  - [🧭 Índice](#-índice)
    - [📝 Formato Markdown útil:](#-formato-markdown-útil)
  - [1️⃣ Introducción](#1️⃣-introducción)
  - [Importancia de la semantica en HTML](#importancia-de-la-semantica-en-html)
    - [¿Por qué es importante usar HTML semantico?](#por-qué-es-importante-usar-html-semantico)
      - [¿Qué es HTML semántico?](#qué-es-html-semántico)
    - [📌 ¿Qué es la jerarquía estructural en HTML?](#-qué-es-la-jerarquía-estructural-en-html)
    - [¿Cúal es la diferencia entre presentación y semantica HTML?](#cúal-es-la-diferencia-entre-presentación-y-semantica-html)
      - [1️⃣ ¿Qué es HTML Presentacional?](#1️⃣-qué-es-html-presentacional)
      - [2️⃣ ¿Qué es HTML Semántico?](#2️⃣-qué-es-html-semántico)
  - [Comprender elementos semánticos matizados](#comprender-elementos-semánticos-matizados)
    - [¿Cuándo se debe utilizar el elemento de énfasis en lugar del elemento de texto idiomático?](#cuándo-se-debe-utilizar-el-elemento-de-énfasis-en-lugar-del-elemento-de-texto-idiomático)
      - [Diferencia entre  y ](#diferencia-entre--y-)
    - [¿Cuándo conviene utilizar el elemento fuerte en lugar del elemento llamar la atención?](#cuándo-conviene-utilizar-el-elemento-fuerte-en-lugar-del-elemento-llamar-la-atención)
    - [¿Qué son las listas de descripciones y cuándo debería utilizarlas?](#qué-son-las-listas-de-descripciones-y-cuándo-debería-utilizarlas)
  - [Trabajando con elementos semánticos de texto y tiempo](#trabajando-con-elementos-semánticos-de-texto-y-tiempo)
    - [¿Cómo funcionan las comillas en bloque y en línea en HTML?](#cómo-funcionan-las-comillas-en-bloque-y-en-línea-en-html)
      - [1. ¿Qué es una cita en HTML?](#1-qué-es-una-cita-en-html)
    - [¿Cómo se muestran las abreviaturas en HTML?](#cómo-se-muestran-las-abreviaturas-en-html)
      - [1️⃣ Acronym (Acrónimo)](#1️⃣-acronym-acrónimo)
      - [2️⃣ Initialism (Inicialismo)](#2️⃣-initialism-inicialismo)
    - [¿Cómo se muestran direcciones en HTML?](#cómo-se-muestran-direcciones-en-html)
    - [How Do You Display Times and Dates in HTML?](#how-do-you-display-times-and-dates-in-html)
  - [Trabajar con elementos semánticos especializados](#trabajar-con-elementos-semánticos-especializados)
    - [How Do You Display Mathematical Equations and Chemical Formulas in HTML?](#how-do-you-display-mathematical-equations-and-chemical-formulas-in-html)
    - [How Do You Represent Computer Code in HTML?](#how-do-you-represent-computer-code-in-html)

### 📝 Formato Markdown útil:
- **Negrita**
- *Itálica*
- ***Negrita e itálica***
- ~~Texto tachado~~  

---

## 1️⃣ Introducción
La semántica en HTML se refiere al uso de etiquetas que describen claramente el significado del contenido que contienen. En lugar de utilizar únicamente etiquetas genéricas como `<div>` o `<span>`, la semántica propone emplear elementos que indiquen el propósito del contenido dentro de la estructura de una página web.

HTML5 introdujo varias etiquetas semánticas que permiten organizar mejor la información, facilitando la comprensión tanto para los desarrolladores como para los navegadores, motores de búsqueda y tecnologías de accesibilidad. Algunas de estas etiquetas son `<header>`, `<nav>`, `<section>`, `<article>`, `<aside> `y `<footer>`.

El uso adecuado de etiquetas semánticas mejora la estructura del documento, optimiza el posicionamiento en buscadores (SEO) y hace que el contenido sea más accesible para personas que utilizan lectores de pantalla. En resumen, la semántica en HTML permite crear páginas web más organizadas, comprensibles y profesionales.

## Importancia de la semantica en HTML

### ¿Por qué es importante usar HTML semantico?

Semántica se refiere al significado de palabras o elementos dentro de un lenguaje.

En HTML, significa que cada etiqueta tiene un propósito y significado específico, no solo una función visual.

Ejemplo:

`<p>Este es un párrafo</p>`


La etiqueta` <p> `significa párrafo.
No solo cambia el estilo, sino que indica que el contenido es un bloque de texto.

#### ¿Qué es HTML semántico?

Es usar etiquetas que describan claramente qué es el contenido.

En lugar de hacer esto:
`<div>Menú</div>`

Se recomienda hacer esto: `<nav>Menú</nav>`

Porque <nav> indica que es navegación.

📌 ¿Por qué es importante usar HTML semántico?

Hay 3 razones principales:

1. Mejora la accesibilidad
Los lectores de pantalla (para personas con discapacidad visual) entienden mejor la estructura del sitio.

2. Mejora el SEO
Google entiende mejor tu página si usas etiquetas correctas.
Eso ayuda a posicionar mejor en buscadores.

3. Mejora la experiencia del desarrollador
Es más fácil leer y mantener el código.
Sabes rápidamente dónde está el header, el nav, el footer, etc.h


### 📌 ¿Qué es la jerarquía estructural en HTML?

Es el orden correcto de los encabezados:
h1 → h2 → h3 → h4 → h5 → h6

Funciona como los títulos en un documento de Word:
- h1 → Título principal
- h2 → Subtítulo
- h3 → Sub-subtítulo
- No debes saltarte niveles.

❌ **Incorrecto**:

<h1>Título</h1>
<h3>Subtema</h3>


✅ **Correcto**:

<h1>Título</h1>
<h2>Subtema</h2>
<h3>Detalle</h3>

**¿Por qué es importante la jerarquía?**
Hay 3 razones principales:

1. Accesibilidad
Los lectores de pantalla usan los encabezados para navegar la página.
Si saltas de h1 a h3, el usuario puede pensar que falta contenido.

2. SEO
Google usa los encabezados para entender la estructura del contenido.
Si están mal ordenados, tu página puede posicionar peor.

3. Navegadores
Si el HTML está mal estructurado, el navegador "adivina" lo que quisiste hacer.
Eso puede causar errores visuales o problemas técnicos.

### ¿Cúal es la diferencia entre presentación y semantica HTML?

#### 1️⃣ ¿Qué es HTML Presentacional?

Es el HTML que solo cambia la apariencia (cómo se ve el contenido).
Antes se usaban etiquetas como:

- `<font>`
- `<center>`
- `<big>`

Ejemplo:
```HTML
<font size="5" color="blue">Texto azul</font>
```

🔴 Problema:
- Mezcla contenido con estilo
- No es accesible
- No es buena práctica moderna
- Está deprecated (ya no recomendado)

Hoy en día el estilo SIEMPRE se hace con CSS, no con HTML.

#### 2️⃣ ¿Qué es HTML Semántico?

Es el HTML que describe el significado del contenido.

No dice cómo se ve.
Dice qué es.

Ejemplos modernos:

- `<header>` → encabezado
- `<nav>` → navegación
- `<section>` → sección
- `<article>` → contenido independiente
- `<figure>` → imagen o ilustración

Ejemplo:
```HTML
<header>
  <nav>
    <a href="#">Home</a>
    <a href="#">About</a>
  </nav>
</header>
```
 Ventajas:
- Mejor para SEO (Google entiende mejor tu web)
- Mejor para accesibilidad (screen readers)
- Código más limpio
- Más profesional

**Palabras en Ingles**
- understanding = Comprender
- Nuanced = matizados
- Closely → De cerca / Estrechamente
- Display → Mostrar / Pantalla / Exhibir
- Highlighting → Resaltando / Destacando
- Thoughts → Pensamientos
- Spec (Specification) → Especificación
- Somehow → De alguna manera
- Surrounding → Alrededor de / Circundante
- Italicized → En cursiva
- Conveys → Transmite / Expresa
- Instead → En lugar de
- Bring → Traer / Llevar
- Commonly → Comúnmente / Habitualmente
- Summaries → Resúmenes
- Boldface → Negrita / Tipo de letra en negrita
- Renders → Renderiza / Muestra / Representa
- Bold text → Texto en negrita
- Uncommenting → Descomentar (quitar un comentario en código)
- Wraps → Envuelve / Rodea / Ajusta (según contexto, por ejemplo texto que se ajusta)
- Sheets → Hojas
- Slightly → Ligeramente / Un poco
- Towards → Hacia
- Distinguish → Distinguir
- Them → Ellos / Ellas / Los / Las (depende del contexto

## Comprender elementos semánticos matizados
### ¿Cuándo se debe utilizar el elemento de énfasis en lugar del elemento de texto idiomático?

#### Diferencia entre <i> y <em>
Aunque se ven iguales (italics) en el navegador, NO significan lo mismo.
 <i> — Idiomatic Text

Antes era solo para poner texto en cursiva.
Pero ahora se usa para:
- Frases en otro idioma
- Pensamientos
- Términos técnicos
- Voz diferente o especial
- Expresiones idiomáticas

Ejemplo:
```HTML
<p>There is a certain <i lang="fr">je ne sais quoi</i> in the air.</p>
```

Aquí:
- No es algo importante.
- Solo es una frase en francés.
- Es diferente al resto del texto.

 `<i>` NO indica importancia.

`<em>` — Emphasis (Énfasis)

Se usa cuando quieres dar importancia real a una palabra.

Ejemplo:
```HTML
<p>Never give up on <em>your</em> dreams.</p>
```

Aquí cambia el significado:
Sin énfasis: Never give up on your dreams.
Con énfasis: Nunca abandones tus sueños (no los de otros).

 `<em> `SÍ agrega importancia semántica.

Los lectores de pantalla incluso lo leen con más énfasis.

### ¿Cuándo conviene utilizar el elemento fuerte en lugar del elemento llamar la atención?
Diferencia entre `<b> y <strong>`
Aunque ambos se ven en negrita, no significan lo mismo.

**`<b>` — Bring Attention To**

Se usa para:
- Resaltar palabras clave
- Nombres de productos
- Palabras importantes visualmente
- Sin indicar urgencia o importancia real

Ejemplo:
```HTML
<p>El producto <b>SuperSound 3000</b> tiene buena calidad.</p>
```

Solo llama la atención.
No indica urgencia ni importancia semántica.

**`<strong>` — Importancia o urgencia**

Se usa cuando el texto es:
- Muy importante
- Urgente
- Advertencia
- Crítico
Ejemplo:
```HTML
<p><strong>Warning:</strong> This product may cause allergic reactions.</p>
```

 Aquí sí hay importancia real.
 Los lectores de pantalla lo leen con más énfasis.

🎯 Regla fácil
|Elemento|Significado|
|----------|-------------|
|`<b>`|	Solo llama la atención|
|`<strong>`|	Texto importante o urgente|

### ¿Qué son las listas de descripciones y cuándo debería utilizarlas?
Qué es una Description List?
Es una lista especial para mostrar:

- Término → Descripción
- Clave → Valor
- Concepto → Definición

Se usa cuando tienes pares relacionados de información.
 Estructura básica

Hay 3 etiquetas:
```html
<dl>   <!-- Contenedor principal -->
  <dt>Termino</dt>   <!-- Description Term -->
  <dd>Descripción</dd>   <!-- Description Details -->
</dl>
```
 Ejemplo tipo diccionario

```html
<dl>
  <dt>HTML</dt>
  <dd>HyperText Markup Language</dd>

  <dt>CSS</dt>
  <dd>Cascading Style Sheets</dd>
</dl>
```
 Ejemplo tipo receta

```html
<dl>
  <dt>Flour</dt>
  <dd>2 cups</dd>

  <dt>Sugar</dt>
  <dd>1/2 cup</dd>
</dl>
```
**¿Cuándo usar <dl>?**
Cuando tienes:

- 📚 Glosarios
- 🛒 Especificaciones de productos
- ❓ Preguntas y respuestas
- 📞 Información de contacto
- 🧾 Metadatos

Cualquier estructura tipo clave → valor

🚨 No confundas con:

- `<ul>` → lista sin orden
- `<ol>` → lista ordenada
- `<li>` → elemento de lista normal

Description list es diferente.

**Palabras en Ingles**

## Trabajando con elementos semánticos de texto y tiempo
### ¿Cómo funcionan las comillas en bloque y en línea en HTML?
#### 1. ¿Qué es una cita en HTML?

Una cita es texto que tomas de otro autor, libro, página web, etc.
En HTML existen dos tipos principales:

- Cita larga → `<blockquote>`

- Cita corta (en línea) → <q>

- 2. `<blockquote>` → Para citas largas

Se usa cuando copias un párrafo completo o varios párrafos de otra fuente.

Ejemplo:
```HTML
<blockquote cite="https://www.freecodecamp.org/news/learn-to-code-book/">
  "Can you imagine what it would be like to be a successful developer?"
</blockquote>
```
✅ ¿Qué hace?

Muestra el texto con una indentación (más hacia la derecha).
Indica que es una cita larga.
Puede tener el atributo cite con la URL de donde salió la cita.

Importante
- El atributo cite="URL":
- NO se muestra visualmente.

Solo ayuda a buscadores y lectores de pantalla.

Blockquote con varios párrafos

Si la cita tiene varios párrafos, puedes usar <p> dentro:

```HTML
<blockquote cite="https://ejemplo.com">
  <p>Primer párrafo.</p>
  <p>Segundo párrafo.</p>
</blockquote>
```

Todos siguen siendo parte de la misma cita.

🔹 3. `<cite>` → Para mostrar el título de la obra

⚠ No confundas:

cite (atributo)

<cite> (elemento HTML)

El elemento <cite> se usa para marcar el título de una obra (libro, canción, película, artículo, etc.).

Ejemplo:
```HTML
<p>—Quincy Larson, <cite>How to Learn to Code and Get a Developer Job</cite></p>

```
Esto muestra visualmente el título (normalmente en cursiva).

🔹 4. <q> → Para citas cortas dentro de un párrafo

Se usa para frases pequeñas dentro del texto.

Ejemplo:
```HTML
<p>
  As Quincy Larson said,
  <q cite="https://www.freecodecamp.org/news/learn-to-code-book/">
    Momentum is everything.
  </q>
</p>
```
¿Qué hace?

Agrega comillas automáticamente.

Mantiene la cita dentro del mismo párrafo.

También puede usar el atributo cite.

🔹 5. Diferencia entre <blockquote> y <q>
|Elemento	|Uso	|Cómo se ve|
|----------|------|--------------|
|<blockquote>	|Citas largas	|Texto indentado
|<q>	|Citas cortas	|Texto con comillas dentro del párrafo

**Palabras en Inglés**

- Quoted → Citado / Entre comillas
- Surrounding → Alrededor de / Rodeando / Circundante
- Mainly → Principalmente / Mayormente
- Quotations → Citas / Comillas
- Cite → Citar / Mencionar 
- Engines → Motores
- Slightly indented → Ligeramente sangrado / Con una pequeña sangría
- Marks → Marcas / Signos
- Wrap → Envolver / Enmarcar 
- Paragraphs → Párrafos
- So far → Hasta ahora / Por ahora
- Inline → En línea 
- Readers → Lectores 

### ¿Cómo se muestran las abreviaturas en HTML?
Una abbreviación (abbreviation) es una forma corta de una palabra o frase.
Ejemplo:

- Dr. = Doctor
- HTML = HyperText Markup Language

🔹 Tipos de abreviaciones

Hay dos tipos principales:

#### 1️⃣ Acronym (Acrónimo)

Se pronuncia como una palabra.

Ejemplo:

GUI → Graphical User Interface
(se pronuncia “gooey”)

#### 2️⃣ Initialism (Inicialismo)

Se pronuncia letra por letra.

Ejemplo:

HTML → HyperText Markup Language
(se pronuncia H-T-M-L)
🔹 ¿Qué elemento HTML se usa?

El elemento correcto es:

`<abbr>`


Sirve para indicar que un texto es una abreviación.

🔹 Ejemplo básico
```HTML
<p><abbr>HTML</abbr> is the foundation of the web.</p>
```

Visualmente no cambia mucho, pero le da significado semántico al texto.

🔹 Usando el atributo title

Si quieres mostrar el significado completo cuando el usuario pase el mouse encima, usas el atributo title.
```HTML
<p>
  <abbr title="HyperText Markup Language">HTML</abbr>
  is the foundation of the web.
</p>
```
✅ ¿Qué pasa aquí?

Cuando el usuario pasa el mouse sobre HTML, aparece un pequeño cuadro (tooltip).

Algunos navegadores muestran una línea punteada debajo.

🔹 ¿Cuándo usar `<abbr>`?

✔ Cuando la abreviación puede no ser clara.
✔ Cuando quieres dar contexto adicional.
✔ Cuando usas la abreviación por primera vez en el texto.

No es obligatorio usarlo siempre, pero es buena práctica.

**Palabras en Inglés**

- Shortened → Acortado / Abreviado
- Acronyms → Acrónimos (siglas que se pronuncian como una palabra, ej: NASA)
- Initialisms → Siglas (se pronuncian letra por letra, ej: HTML o FBI)
- Dotted → Punteado / De puntos (muy común para bordes: border-style: dotted;)
- Small caps → Versalitas (letras mayúsculas con el tamaño de las minúsculas)
- Hovers → Pasar el ratón por encima (el estado :hover en CSS)
- Tooltip → Descripción emergente / Glosa (el cuadrito de texto que sale al dejar el cursor quieto)
- Unclear → Poco claro / Confuso
- Judgment → Juicio / Criterio
- Cluttering → Abarrotar / Desordenar / Llenar de cosas innecesarias



### ¿Cómo se muestran direcciones en HTML?
En HTML, el elemento que se usa para mostrar información de contacto es:

`<address>`

Este elemento es semántico, lo que significa que tiene un significado especial para el navegador y los motores de búsqueda.
Se usa para mostrar:

- 🏢 Nombre de empresa
- 📍 Dirección física
- 📞 Teléfono
- 📧 Correo electrónico
- 👤 Información de contacto de un autor

🔹 Ejemplo básico
```HTML
<address>
  <h2>Company Name</h2>
  <p>
    1234 Elm Street<br>
    Springfield, IL 62701<br>
    United States
  </p>
  <p>Phone: <a href="tel:+15555555555">+1 (555) 555-5555</a></p>
  <p>Email: <a href="mailto:contact@company.com">contact@company.com</a></p>
</address>
```
🔹 Explicación importante
✅ <br>

Se usa para hacer saltos de línea dentro de la dirección.

✅ tel:
<a href="tel:+15555555555">


Permite que el usuario haga clic y llame directamente desde su dispositivo (especialmente en celulares).

✅ mailto:
<a href="mailto:contact@company.com">


Abre el cliente de correo del usuario para enviar un email.

🔹 Desventaja de mailto

Uno de los problemas es que:
Puede ser usado por spammers.
Algunos usuarios lo consideran inseguro o molesto.
🔹 ¿Por qué usar <address> en lugar de <div>?
Porque <address>:
Tiene significado semántico.
Mejora la accesibilidad.
Es mejor práctica en desarrollo web.

### How Do You Display Times and Dates in HTML?
En HTML, el elemento que se usa para representar fechas y horas es:
`<time>`

Sirve para mostrar momentos específicos como:
- 📅 Fechas
- ⏰ Horas
- 📆 Eventos
- 🎓 Fechas de graduación
- 📰 Fechas de publicación

🔹 Ejemplo con hora
`<p>The reservations are for <time datetime="20:00">20:00</time></p>`

✅ ¿Qué hace datetime?

El atributo datetime:
Traduce la fecha u hora a un formato que las máquinas pueden entender.
Ayuda a los motores de búsqueda.
Ayuda al navegador a procesar mejor la información.
🔹 Ejemplo con fecha y hora

```HTML
<p>
  The graduation will be on 
  <time datetime="2024-06-15T15:00">June 15</time>
</p>
```
🔹 Formato ISO 8601

El valor del atributo datetime debe seguir el formato internacional ISO 8601:

YYYY-MM-DDTHH:MM:SS


Ejemplo:

2024-06-15T15:00:00

🔎 Explicación:
2024 → Año
06 → Mes
15 → Día
T → Separador entre fecha y hora
15:00 → Hora en formato 24 horas (3 PM)

🔹 ¿Qué significa la "T"?
La T es simplemente el separador entre:
Fecha
Hora

🔹 ¿Cuándo usar <time>?

✔ Para eventos
✔ Para publicaciones
✔ Para citas
✔ Para recordatorios
✔ Para sistemas que procesen fechas automáticamente

Es buena práctica usarlo cuando una fecha tenga importancia estructural.

## Trabajar con elementos semánticos especializados



**Palabras en Inglés**
- Superscript → Superíndice 
- Slightly higher → Ligeramente más alto 
- Superior lettering → Letras superiores 
### How Do You Display Mathematical Equations and Chemical Formulas in HTML?

En HTML existen dos elementos especiales para mostrar texto arriba o abajo de la línea normal:

- <sup> → Superscript (superíndice)
- <sub> → Subscript (subíndice)
-  <sup> – Superscript (superíndice)

Se usa para mostrar texto más pequeño y arriba de la línea normal.

Ejemplo con exponentes:
```html
<p>2<sup>2</sup> (2 squared) is 4.</p>
```

🔎 Aquí:

El segundo 2 está dentro de `<sup>.`

Se ve pequeño y elevado.

Representa 2².

📌 Usos comunes de` <sup>`

✔ Exponentes → 10`<sup>`3`</sup>`
✔ Números ordinales → 1`<sup>st</sup>`, 2`<sup>nd</sup>`
✔ Abreviaciones especiales

Ejemplo:
```html
<p>Monseigneur is written as M<sup>gr</sup>.</p>

```
⚠ IMPORTANTE:

El elemento `<sup>` debe usarse solo cuando el texto realmente tenga significado como superíndice.

👉 Si solo quieres subir texto por diseño, debes usar CSS, no <sup>.

🔹 2️⃣` <sub>` – Subscript (subíndice)

Se usa para mostrar texto más pequeño y abajo de la línea normal.

Ejemplo con fórmula química:
```html
<p>CO<sub>2</sub></p>
```

🔎 Aquí:

El número 2 está abajo.

Representa dióxido de carbono.

📌 Usos comunes de `<sub>`

✔ Fórmulas químicas → H`<sub>2</sub>O`
✔ Variables matemáticas
✔ Notas al pie

🔹 Diferencia rápida
Elemento	Posición	Uso
<sup>	Arriba	Exponentes, ordinales
<sub>	Abajo	Fórmulas químicas
✅ Respuestas Correctas
1️⃣ What is the primary use of the superscript element?

✔ To display text as a superscript above the normal line of text.

2️⃣ Which example is correct?

✔

<p>2<sup>2</sup> (2 squared) is 4.</p>

3️⃣ What should be used instead if text is raised only for styling?

✔ CSS



**Palabras en Inglés**

- Snippets → Fragmentos de código 
- Monospaced font → Fuente monoespaciada 
- Mindful → Consciente / Atento 
- Indented several → Sangrado varias veces 
- Indentation → Sangría / Sangrado 

### How Do You Represent Computer Code in HTML?

Cuando quieres mostrar código dentro de una página web, HTML tiene dos elementos importantes:

- 🔹 <code> → Para código corto en línea

- 🔹 <pre> → Para texto preformateado (bloques largos de código)

- 🔹 1️⃣ <code> – Código en línea

Se usa para mostrar pequeños fragmentos de código dentro de un párrafo.

Ejemplo:
```html
<p>
  To change text color in CSS use 
  <code>color: blue;</code>
</p>
```
✅ ¿Qué hace?

Indica que el texto es código.
El navegador lo muestra con fuente monoespaciada (como Consolas o Courier).
Es ideal para una sola línea.

` <pre>` – Texto preformateado

Se usa cuando quieres mostrar varias líneas de código.

Ejemplo:
```html
<pre>
  <code>
    body {
      color: red;
    }
  </code>
</pre>
```
✅ ¿Qué hace <pre>?

Respeta los espacios.

Respeta los saltos de línea.

Muestra el texto exactamente como está escrito en el HTML.

⚠ Muy importante:
Si agregas espacios o indentación, el navegador los mostrará.

🔹 Diferencia rápida
Elemento	Uso
- <code>	Código corto dentro de texto
- <pre>	Bloques largos de código
- <pre> + <code>	Forma correcta para mostrar bloques de código
🔹 Estilo por defecto de <code>

✔ Fuente monoespaciada (monospaced font)

No es:

Negrita

Cursiva

Subrayado