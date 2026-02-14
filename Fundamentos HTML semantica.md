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