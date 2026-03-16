# 📘 Manual de Forms y Tables
_Apuntes diarios y ejemplos prácticos_

---

## 📌 Información general

| Campo | Detalle |
|------|--------|
| Autor | Carlos Sancir |
| Fecha inicio | 9/3/2026 |
| Objetivo | Aprender HTML desde cero |
| Nivel | Básico → Avanzado |

---
- [📘 Manual de Forms y Tables](#-manual-de-forms-y-tables)
  - [📌 Información general](#-información-general)
  - [Trabajar con Forms](#trabajar-con-forms)
    - [Como hacer forms, Labels y Inputs trabajando en HTML](#como-hacer-forms-labels-y-inputs-trabajando-en-html)
      - [Formularios, Labels e Inputs en HTML](#formularios-labels-e-inputs-en-html)
      - [**El elemento `<input>`**](#el-elemento-input)
      - [El elemento `<label>`](#el-elemento-label)
      - [Asociación explícita (usando `for` e `id`)](#asociación-explícita-usando-for-e-id)
    - [Tipos de Botones en HTML](#tipos-de-botones-en-html)
      - [El elemento `<button>`](#el-elemento-button)
      - [Los 3 tipos de botones (`type`)](#los-3-tipos-de-botones-type)
    - [Validación de Formularios en el Cliente (Client-Side Validation)](#validación-de-formularios-en-el-cliente-client-side-validation)
      - [¿Qué es la validación?](#qué-es-la-validación)
    - [3. `minlength` y `maxlength` — Longitud mínima y máxima](#3-minlength-y-maxlength--longitud-mínima-y-máxima)
  - [Ejemplo completo con todas las validaciones](#ejemplo-completo-con-todas-las-validaciones)
  - [Resumen de atributos de validación](#resumen-de-atributos-de-validación)
  - [Respuestas a las preguntas de repaso](#respuestas-a-las-preguntas-de-repaso)
    - [What Are the Different Form States, and Why Are They Important?](#what-are-the-different-form-states-and-why-are-they-important)
      - [Estados de los Formularios en HTML (Form States)](#estados-de-los-formularios-en-html-form-states)
  - [Respuestas a las preguntas de repaso](#respuestas-a-las-preguntas-de-repaso-1)
  - [Trabajar con Tables](#trabajar-con-tables)
    - [¿Para qué se utilizan las tablas HTML y para qué no se deberían utilizar?](#para-qué-se-utilizan-las-tablas-html-y-para-qué-no-se-deberían-utilizar)
      - [¿Para qué sirven las tablas?](#para-qué-sirven-las-tablas)
      - [Jerarquía de una tabla](#jerarquía-de-una-tabla)
  - [¿Tablas vs Divs?](#tablas-vs-divs)
  - [Respuestas a las preguntas de repaso](#respuestas-a-las-preguntas-de-repaso-2)
  - [Trabajar con herramientas HTML](#trabajar-con-herramientas-html)
    - [¿Qué es un validador HTML y cómo puede ayudarle a depurar su código?](#qué-es-un-validador-html-y-cómo-puede-ayudarle-a-depurar-su-código)
      - [Validadores HTML (HTML Validators)](#validadores-html-html-validators)
      - [¿Por qué HTML es "perdonador"?](#por-qué-html-es-perdonador)
      - [¿Cuándo puede salir mal?](#cuándo-puede-salir-mal)
      - [¿Qué es un validador HTML?](#qué-es-un-validador-html)
      - [Beneficios:](#beneficios)
      - [Validadores más usados](#validadores-más-usados)
      - [1. W3.org — El más reconocido](#1-w3org--el-más-reconocido)
      - [2. JSONFormatter](#2-jsonformatter)
  - [Ejemplo de error que un validador detectaría](#ejemplo-de-error-que-un-validador-detectaría)
  - [Resumen](#resumen)
  - [Respuestas a las preguntas de repaso](#respuestas-a-las-preguntas-de-repaso-3)
    - [DOM Inspector y DevTools](#dom-inspector-y-devtools)
      - [Conceptos clave](#conceptos-clave)
      - [¿Qué es el DOM?](#qué-es-el-dom)
      - [¿Cómo abrir las DevTools?](#cómo-abrir-las-devtools)


## Trabajar con Forms
**Palabras en ingles**
Gather: Reunir / Recolectar (ej. recolectar datos).

-Such as: Tales como / Como por ejemplo.
- Upon submission: Al enviar / Tras el envío (usado mucho en formularios).
- Enable: Activar / Habilitar.
- Typing: Escribiendo / Tecleando.
- By nesting: Al anidar / Mediante el anidamiento (común en programación o carpetas).
- Understood: Entendido / Comprendido.
- Hints: Pistas / Sugerencias.
- Placeholder: Marcador de posición (el texto gris que sale en un cuadro antes de escribir).
- Go away: Desaparecer / Irse.
### Como hacer forms, Labels y Inputs trabajando en HTML

#### Formularios, Labels e Inputs en HTML

**¿Qué es un formulario (`<form>`)?**
El elemento `<form>` se usa para **recopilar información del usuario**, como nombres, correos electrónicos, contraseñas, etc.

```html
<form action="url-destino">
  <!-- aquí van los elementos de entrada -->
</form>
```

> El atributo `action` indica **a dónde se enviarán los datos** cuando el usuario envíe el formulario.

---
#### **El elemento `<input>`**

El elemento `<input>` permite al usuario **ingresar datos**. Es un elemento vacío (no tiene etiqueta de cierre).

```html
<form action="">
  <input type="text" />
</form>
```

El atributo `type` define **qué tipo de dato** se espera:

| Valor de `type` | Descripción |
|-----------------|-------------|
| `text`          | Texto libre |
| `email`         | Dirección de correo electrónico |
| `password`      | Contraseña (oculta el texto) |
| `number`        | Solo números |
| `submit`        | Botón para enviar el formulario |

---

#### El elemento `<label>`

El `<label>` proporciona una **descripción visible** para un campo de entrada. Mejora la accesibilidad del formulario.

**Asociación implícita (anidando el input dentro del label)**

```html
<form action="">
  <label>
    Nombre Completo:
    <input type="text" />
  </label>
</form>
```

> Al hacer clic en el texto "Nombre Completo:", el cursor se posiciona automáticamente en el campo de entrada.

#### Asociación explícita (usando `for` e `id`)

```html
<form action="">
  <label for="email">Correo Electrónico:</label>
  <input type="email" id="email" />
</form>
```

> ⚠️ El valor del atributo `for` en el `<label>` debe ser **igual** al valor del atributo `id` en el `<input>`.

---

**El atributo `placeholder`**

El `placeholder` muestra un **texto de ayuda** dentro del campo antes de que el usuario escriba algo. Desaparece al comenzar a escribir.

```html
<form action="">
  <label for="email">Correo Electrónico:</label>
  <input type="email" id="email" placeholder="ejemplo@correo.com" />
</form>
```

> Usa el `placeholder` para mostrar el **formato esperado** del dato (no como sustituto del label).

---

**Ejemplo completo**

```html
<form action="/enviar-datos">

  <label for="nombre">Nombre:</label>
  <input type="text" id="nombre" placeholder="Juan Pérez" />

  <label for="correo">Correo:</label>
  <input type="email" id="correo" placeholder="juan@ejemplo.com" />

  <input type="submit" value="Enviar" />

</form>
```

---

**Resumen de conceptos clave**

| Concepto | Descripción |
|----------|-------------|
| `<form action="">` | Contenedor del formulario; `action` define el destino de los datos |
| `<input type="">` | Campo de entrada; `type` define el tipo de dato esperado |
| `<label>` implícito | El `<input>` se anida dentro del `<label>` |
| `<label for="">` explícito | El `for` del label debe coincidir con el `id` del input |
| `placeholder` | Texto de ayuda dentro del campo (desaparece al escribir) |

---

Respuestas a preguntas de repaso

1. **¿Para qué sirve el atributo `for` en un `<label>`?**
   → Para **asociar explícitamente** un label con su input correspondiente.

2. **¿Cuál es un valor válido para el atributo `type` de un input?**
   → `text`

3. **¿Para qué sirve el atributo `placeholder`?**
   → Para mostrar **un texto de ejemplo o pista** dentro del campo de entrada.


### Tipos de Botones en HTML

#### El elemento `<button>`

Se usa para ejecutar una acción cuando el usuario hace clic.

```html
<button>Start Game</button>
```

---

#### Los 3 tipos de botones (`type`)

**1. `type="button"` — Botón genérico**

No hace nada solo, necesita JavaScript para funcionar.

```html
<button type="button">Mostrar Alerta</button>
```

**1. `type="submit"` — Enviar formulario**

Envía los datos del formulario al servidor.

```html
<form action="">
  <label for="email">Email:</label>
  <input type="email" id="email" name="email" />
  <button type="submit">Enviar</button>
</form>
```

**1. `type="reset"` — Limpiar formulario**

Borra todos los datos que el usuario escribió.

```html
<button type="reset">Limpiar</button>
```

> ⚠️ No se recomienda usar reset — el usuario podría borrar todo por accidente.

---

**`<button>` vs `<input type="button">`**

| | `<button>` | `<input type="button">` |
|---|---|---|
| ¿Puede tener texto? | ✅ | ✅ (con `value`) |
| ¿Puede tener imágenes/iconos dentro? | ✅ | ❌ |
| ¿Es elemento vacío? | ❌ | ✅ |

```html
<!-- input: solo texto con value -->
<input type="button" value="Start Game" />

<!-- button: puede tener texto, iconos, imágenes -->
<button type="button">🎮 Start Game</button>
```

---

**Resumen de valores para `type`**

| Valor | ¿Qué hace? |
|-------|------------|
| `button` | Nada por defecto, requiere JavaScript |
| `submit` | Envía los datos del formulario |
| `reset` | Limpia todos los campos del formulario |

---
**Biblioteca de Ingles**
- Clear out all: Limpiar todo / Vaciar por completo.
- Lead: Guiar / Dirigir / Liderar.
- Clutter up: Desordenar / Amontonar / Llenar de trastos 



### Validación de Formularios en el Cliente (Client-Side Validation)

#### ¿Qué es la validación?

Cuando un usuario llena un formulario, es importante que ingrese la información correcta antes de enviarla. HTML tiene validaciones **integradas** que detectan errores automáticamente.

---

**Client-Side vs Server-Side**

| | Client-Side | Server-Side |
|---|---|---|
| ¿Dónde ocurre? | En el navegador del usuario | En el servidor |
| ¿Para qué sirve? | Detectar errores antes de enviar | Seguridad y procesamiento de datos |
| ¿Es suficiente sola? | ❌ No | ✅ Siempre necesaria |

> ⚠️ La validación del lado del cliente **no es suficiente** por sí sola. Los usuarios maliciosos pueden saltársela, por eso también se necesita validación del lado del servidor.

---

**Tipos de validación en HTML**

**1. `required` — Campo obligatorio**

Obliga al usuario a llenar ese campo antes de enviar el formulario.

```html
<form action="">
  <label for="email">Email (campo obligatorio):</label>
  <input required type="email" name="email" id="email" />
  <button type="submit">Enviar</button>
</form>
```

> Si el usuario intenta enviar sin llenar el campo, el navegador muestra un mensaje de alerta automáticamente.

---

**2. Validación de formato en `type="email"`**

El tipo `email` valida automáticamente que el formato sea correcto (debe incluir `@`).

```html
<input required type="email" name="email" id="email" />
```

> Si el usuario escribe `abc` y envía, el navegador alerta que falta el símbolo `@`.

---

### 3. `minlength` y `maxlength` — Longitud mínima y máxima

Controlan cuántos caracteres debe tener el valor ingresado.

```html
<form action="">
  <label for="email">Email (campo obligatorio):</label>
  <input
    required
    type="email"
    name="email"
    id="email"
    minlength="4"
    maxlength="64"
  />
  <button type="submit">Enviar</button>
</form>
```

| Atributo | ¿Qué hace? |
|----------|------------|
| `minlength="4"` | El valor debe tener al menos 4 caracteres |
| `maxlength="64"` | El valor no puede superar 64 caracteres |

> Si escribes `b@m` (3 caracteres) e intentas enviar, el navegador avisa que no cumple el mínimo.

---

## Ejemplo completo con todas las validaciones

```html
<form action="">
  <label for="email">Correo Electrónico:</label>
  <input
    required
    type="email"
    id="email"
    name="email"
    minlength="4"
    maxlength="64"
    placeholder="ejemplo@correo.com"
  />
  <button type="submit">Enviar formulario</button>
</form>
```

---

## Resumen de atributos de validación

| Atributo | ¿Qué valida? |
|----------|-------------|
| `required` | Que el campo no esté vacío |
| `type="email"` | Que el formato tenga `@` y sea un email válido |
| `minlength` | Que el texto tenga un mínimo de caracteres |
| `maxlength` | Que el texto no supere un máximo de caracteres |

---

## Respuestas a las preguntas de repaso

1. **¿Para qué sirven `minlength` y `maxlength`?**
   → Para **establecer la longitud mínima y máxima en caracteres** del campo de entrada.

2. **¿Qué atributo marca un campo como obligatorio?**
   → El atributo **`required`**.

3. **¿Qué pasa si envías un email sin el símbolo `@`?**
   → El navegador **muestra un mensaje de alerta** indicando que falta el `@`.

**Biblioteca en Ingles**
- Client-side: Lado del cliente (todo lo que ocurre en el navegador del usuario).
- Features: Funciones / Características / Funcionalidades.
- Handling requests: Manejo de peticiones / Gestión de solicitudes.
- Server-side: Lado del servidor (todo lo que ocurre en la computadora remota/base de datos).
- Measures: Medidas (como en "medidas de seguridad").
- Gets submitted: Se envía / Es enviado (referente a un formulario o datos).
- Pop up: Ventana emergente / Mensaje emergente.

**Palabra en Ingles**
- Read-only: Solo lectura (cuando un archivo o campo no se puede editar).
- Whitespace: Espacio en blanco (se refiere a los espacios, sangrías o saltos de línea en un documento o código).
- Smooth: Suave / Fluido (usado para describir transiciones, a
### What Are the Different Form States, and Why Are They Important?

####  Estados de los Formularios en HTML (Form States)

Los controles de formulario como los `<input>` pueden estar en diferentes **estados o condiciones**.

---

**1. Estado `default` — Por defecto**

Es como luce el input cuando se carga la página por primera vez. Sin ninguna interacción.

```html
<input type="email" name="email" id="email" />
```

> Un campo en blanco, listo para recibir datos.

---

**2. Estado `focused` — Enfocado**

Ocurre cuando el usuario **hace clic** en el input o lo selecciona con la tecla `Tab`.

```html
<input type="email" name="email" id="email" />
```

> La mayoría de los navegadores muestran un **borde azul** alrededor del input cuando está en foco. Se puede personalizar con CSS.

---

**3. Estado `disabled` — Deshabilitado**

El input **no puede ser clickeado ni activado** por el usuario.

```html
<input disabled type="email" name="email" id="email" />
```

> El campo aparece visualmente apagado/grisáceo. No se puede enfocar ni editar.

---

**4. Estado `readonly` — Solo lectura**

El input **muestra un valor pero no puede ser editado** por el usuario. Se usa el atributo `value` para mostrar el contenido.

```html
<input
  readonly
  type="email"
  name="email"
  id="email"
  value="example@email.com"
/>
```

> El usuario puede **ver y copiar** el valor, pero no modificarlo.

---

**Diferencia clave: `disabled` vs `readonly`**

| | `disabled` | `readonly` |
|---|---|---|
| ¿Se puede enfocar? | ❌ No | ✅ Sí |
| ¿Se puede editar? | ❌ No | ❌ No |
| ¿Se envía al servidor? | ❌ No | ✅ Sí |
| ¿Visualmente apagado? | ✅ Sí | ❌ No |

---
**Resumen de todos los estados**

| Estado | ¿Cómo se activa? | ¿Qué muestra? |
|--------|-----------------|---------------|
| `default` | Al cargar la página | Campo vacío normal |
| `focused` | Al hacer clic o presionar `Tab` | Borde resaltado (azul) |
| `disabled` | Atributo `disabled` | Campo grisáceo, no interactuable |
| `readonly` | Atributo `readonly` | Campo con valor fijo, no editable |

---

**¿Por qué son importantes los estados?**

Porque mejoran la **experiencia del usuario** al:
- Dar retroalimentación visual clara
- Guiar al usuario sobre qué campos puede o no editar
- Prevenir errores antes de enviar el formulario

---

## Respuestas a las preguntas de repaso

1. **¿Qué atributo se usa para deshabilitar un input?**
   → **`disabled`**

2. **¿Qué atributo marca un input como solo lectura?**
   → **`readonly`**

3. **¿Cuándo ocurre el estado `focused`?**
   → Cuando el usuario **hace clic en el input o lo selecciona con la tecla `Tab`**.


## Trabajar con Tables
###  ¿Para qué se utilizan las tablas HTML y para qué no se deberían utilizar?



#### ¿Para qué sirven las tablas?

Las tablas HTML se usan para **mostrar datos tabulares** (información organizada en filas y columnas). Son una de las formas más antiguas de mostrar datos en un navegador (desde los años 90).

> ⚠️ Las tablas **NO deben usarse** para diseñar el layout de una página. Para eso se usa **CSS Flexbox y Grid**.

---

#### Jerarquía de una tabla

```html
<table>
│
├── <thead>  → Encabezado de la tabla
│     └── <tr>  → Fila
│           └── <th>  → Celda de título
│
├── <tbody>  → Cuerpo de la tabla
│     └── <tr>  → Fila
│           ├── <th>  → Celda de encabezado de fila
│           └── <td>  → Celda de dato
│
└── <tfoot>  → Pie de la tabla
      └── <tr>  → Fila
            └── <th>  → Celda de pie
```

---

**Elementos principales**

| Elemento | ¿Qué es? |
|----------|----------|
| `<table>` | Contenedor principal de la tabla |
| `<thead>` | Sección de encabezado |
| `<tbody>` | Sección del cuerpo (los datos) |
| `<tfoot>` | Sección del pie |
| `<tr>` | Fila de la tabla (Table Row) |
| `<th>` | Celda de encabezado (Table Header) |
| `<td>` | Celda de dato (Table Data) |

---

**Tabla mínima con todos los elementos**

```html
<table>
  <thead>
    <tr>
      <th>Título de la tabla</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Primera Fila</th>
      <td>Primer dato</td>
    </tr>
    <tr>
      <th>Segunda Fila</th>
      <td>Segundo dato</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <th>Pie de tabla: autor, fecha, etc.</th>
    </tr>
  </tfoot>
</table>
```

---

**Ejemplo real (Bureau of Labor Statistics)**

```html
<table id="quickfacts">
  <thead>
    <tr>
      <th colspan="2">Datos: Desarrolladores de Software</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Salario Medio 2023</th>
      <td>$130,160 por año</td>
    </tr>
    <tr>
      <th>Educación requerida</th>
      <td>Licenciatura</td>
    </tr>
    <tr>
      <th>Perspectiva laboral 2022-32</th>
      <td>25% (Mucho más rápido que el promedio)</td>
    </tr>
  </tbody>
</table>
```

> El atributo `colspan="2"` hace que una celda ocupe **2 columnas**.

---

## ¿Tablas vs Divs?

Algunos desarrolladores usan `<div>` para imitar tablas, pero:

| | `<table>` | `<div>` |
|---|---|---|
| ¿Semánticamente correcto? | ✅ Sí | ❌ No |
| ¿Recomendado para datos? | ✅ Sí | ❌ No |
| ¿Para layouts de página? | ❌ No | ❌ No (usar CSS Grid/Flexbox) |

---

## Respuestas a las preguntas de repaso

1. **¿Qué elementos están dentro de un `<tr>`?**
   → **`<td>` y `<th>`**

2. **¿Cuáles son las secciones principales de una tabla HTML?**
   → **`<thead>`, `<tbody>` y `<tfoot>`**

3. **¿Para qué se recomiendan las tablas HTML hoy en día?**
   → **Para mostrar datos tabulares** (no para layouts de página).

**Diccionario**

- Still: Todavía / Aún / No obstante (dependiendo de si indica tiempo o contraste).
- Earliest ways: Las formas más antiguas / Los primeros métodos.
- Way back: Mucho tiempo atrás / Hace mucho tiempo.
- Hierarchy: Jerarquía (estructura de niveles, como un árbol genealógico o de carpetas).
- Instead: En su lugar / En vez de ello.
- Might: Podría / Puede que (indica posibilidad).
- Non-data: No relacionado con datos / Información que no son datos puros (como metadatos o formato).
- Depth: Profundidad (en programación, se refiere a qué tan "profundo" llega una rama en una estructura).


## Trabajar con herramientas HTML

### ¿Qué es un validador HTML y cómo puede ayudarle a depurar su código?

#### Validadores HTML (HTML Validators)

#### ¿Por qué HTML es "perdonador"?

HTML es un lenguaje muy tolerante — los elementos se renderizan **incluso cuando cometes errores**, como olvidar una etiqueta de cierre.

```html
<!-- Este h2 no tiene etiqueta de cierre -->
<h2>Subheading 3
```

> El navegador lo renderiza igual gracias a su **algoritmo de parseo**, que detecta errores comunes e intenta mostrar el HTML lo más cercano posible a la intención del autor.

---

#### ¿Cuándo puede salir mal?

El comportamiento "perdonador" puede causar problemas inesperados:

```html
<!-- Este h2 NO tiene etiqueta de cierre -->
<h2>Subheading 3
<p>Este párrafo se renderiza como h2 por error.</p>
```

> El `<p>` hereda el estilo del `<h2>` sin cerrar y se muestra como encabezado en lugar de párrafo. 😱

---

#### ¿Qué es un validador HTML?

Es una herramienta que **verifica si tu código HTML cumple con los estándares oficiales**. Identifica errores y advertencias para asegurarse de que tu página esté correctamente estructurada.

#### Beneficios:
- Detecta errores que el navegador "perdona" pero que pueden causar problemas
- Facilita las revisiones de código en equipo
- Ayuda a colaboradores externos (open-source) a entender tu código
- Asegura compatibilidad con los estándares web

---

#### Validadores más usados

#### 1. W3.org — El más reconocido
**URL:** `validator.w3.org`

Pasos:
1. Visita `validator.w3.org`
2. Haz clic en **"Validate by Direct Input"**
3. Pega tu código HTML
4. Haz clic en **"Check"**
5. Revisa la lista de errores y advertencias

---

#### 2. JSONFormatter
**URL:** `jsonformatter.org`

Pasos:
1. Copia y pega tu HTML en el primer editor
2. Haz clic en **"Validate"**
3. Revisa los errores que aparecen

---

## Ejemplo de error que un validador detectaría

```html
<h1>Artículo</h1>
<p>Introducción del artículo.</p>

<h2>Subtítulo 1</h2>
<p>Contenido del subtítulo 1.</p>

<!-- ❌ Falta la etiqueta de cierre </h2> -->
<h2>Subtítulo 2
<p>Este párrafo se verá como h2 en el navegador.</p>

<!-- ✅ Correcto -->
<h2>Subtítulo 3</h2>
<p>Este párrafo se ve correctamente.</p>
```

---

## Resumen

| Concepto | Descripción |
|----------|-------------|
| HTML perdonador | El navegador renderiza HTML aunque tenga errores |
| Algoritmo de parseo | Mecanismo del navegador que intenta corregir errores automáticamente |
| Validador HTML | Herramienta que verifica si el HTML cumple los estándares |
| W3.org validator | El validador más reconocido y aceptado |

---

## Respuestas a las preguntas de repaso

1. **¿Por qué el navegador renderiza etiquetas aunque haya errores?**
   → Porque el **algoritmo de parseo del navegador** detecta los errores e intenta renderizar las etiquetas como el autor pretendía.

2. **¿Qué es un validador HTML?**
   → Una **herramienta que verifica la validez del código HTML** contra los estándares oficiales.

3. **¿Cuál es un ejemplo de validador HTML?**
   → **W3.org HTML validator**

**Diccionary**
- Forgiving: Tolerante / Flexible (en programación, se refiere a un sistema que no falla aunque cometas pequeños errores).
- Still render: Todavía renderiza / Se sigue mostrando (cuando una web carga a pesar de tener errores).
- Forgetting: Olvidar / Olvidando.
- Backfire: Salir el tiro por la culata / Ser contraproducente.
- Against: En contra de / Contra.
- Anybody: Alguien / Cualquiera.
- Teammates: Compañeros de equipo.
- Widely: Ampliamente / Extensamente (ej. "ampliamente utilizado").


### DOM Inspector y DevTools

#### Conceptos clave

| Término | Definición |
|---------|-----------|
| **Bug** | Un error o problema en el código que hace que no funcione como se espera |
| **Debugging** | El proceso de encontrar y corregir bugs |
| **DOM** | Document Object Model — estructura en forma de árbol que representa los elementos de una página |
| **DevTools** | Herramientas del navegador para inspeccionar HTML, CSS y JavaScript |

---

#### ¿Qué es el DOM?

El **DOM (Document Object Model)** es una representación en forma de árbol de todos los elementos de una página web. Permite a los navegadores y a JavaScript interactuar con el HTML.

```
document
└── <html>
      ├── <head>
      │     └── <title>
      └── <body>
            ├── <h1>
            ├── <p>
            └── <a>
```



---

#### ¿Cómo abrir las DevTools?

| Método | PC | Mac |
|--------|----|-----|
| Clic derecho | Clic derecho → **Inspect** | Clic derecho → **Inspect** |
| Teclado | `Ctrl + Shift + I` | `Cmd + Option + I` |

---

**Pestañas principales de las DevTools**

**1. Pestaña `Elements`**
Muestra la **estructura HTML** de la página. Permite inspeccionar y editar el HTML en tiempo real.

**2. Pestaña `Console`**
Muestra **errores y mensajes** que ocurren en la página. Es la primera pestaña que debes revisar cuando algo no funciona.

---

**Ejemplo de debugging: enlace roto**

```html
<!-- ❌ URL con typo: "larn" en lugar de "learn" -->
<a href="https://www.freecodecamp.org/larn/">freeCodeCamp curriculum</a>

<!-- ✅ URL correcta -->
<a href="https://www.freecodecamp.org/learn/">freeCodeCamp curriculum</a>
```

**Proceso de debugging:**
1. El enlace lleva a una **página 404** (página no encontrada)
2. Abres DevTools → pestaña **Console**
3. Ves el error: `/larn` → 404
4. Identificas el typo: `larn` debería ser `learn`
5. Corriges el `href` → ✅ problema resuelto

> Una **página 404** aparece cuando el servidor no encuentra la URL solicitada.

---

**Flujo de debugging**

```
Encuentras un bug
      ↓
Abres DevTools (Ctrl + Shift + I)
      ↓
Revisas la pestaña Console → errores
      ↓
Revisas la pestaña Elements → estructura HTML
      ↓
Identificas el problema
      ↓
Corriges el código ✅
```

---

**Respuestas a las preguntas de repaso**

1. **¿Cómo se llama el proceso de encontrar y corregir bugs?**
   → **Debugging**

2. **¿Cómo se llama la estructura en forma de árbol que representa los elementos de una página?**
   → **DOM** (Document Object Model)

3. **¿Cuál es el rol de la pestaña "Elements" en las DevTools?**
   → **Muestra la estructura HTML de la página.**

---

## Repaso General — HTML Tables and Forms Review

### Repaso de Elementos y Atributos de Formularios

#### El elemento `<form>`

Se usa para crear un formulario HTML para la entrada del usuario.

```html
<form method="value-goes-here" action="url-goes-here">
  <!-- inputs van aquí -->
</form>
```

| Atributo | ¿Para qué sirve? |
|----------|-----------------|
| `action` | Especifica la URL a donde se envían los datos del formulario |
| `method` | Especifica el método HTTP (GET o POST) |

---

#### El elemento `<input>` y sus atributos

El elemento `<input>` crea un campo de entrada para el usuario.

```html
<!-- Input de texto -->
<input
  type="text"
  id="name"
  name="name"
  placeholder="e.g. Quincy Larson"
  size="20"
  minlength="5"
  maxlength="30"
  required
/>

<!-- Input numérico -->
<input
  type="number"
  id="quantity"
  name="quantity"
  min="2"
  max="10"
  disabled
/>

<!-- Botón -->
<input type="button" value="Show Alert" />
```

**Resumen de atributos del `<input>`**

| Atributo | ¿Qué hace? |
|----------|-----------|
| `type` | Define el tipo de campo: `text`, `email`, `number`, `radio`, `checkbox`, etc. |
| `placeholder` | Muestra una pista/ejemplo dentro del campo antes de escribir |
| `value` | Especifica el valor del input (en botones, define el texto del botón) |
| `name` | Asigna un nombre al campo; en radio buttons, agrupa opciones del mismo nombre |
| `size` | Define el número de caracteres visibles mientras el usuario escribe |
| `min` | Valor mínimo permitido (usado con `type="number"`) |
| `max` | Valor máximo permitido (usado con `type="number"`) |
| `minlength` | Mínimo de caracteres requeridos |
| `maxlength` | Máximo de caracteres permitidos |
| `required` | El campo debe llenarse antes de enviar el formulario |
| `disabled` | El campo queda deshabilitado (no interactuable) |
| `readonly` | El campo es de solo lectura (no editable) |

---

#### El elemento `<label>` y la asociación con inputs

**Asociación implícita** — el input se anida dentro del label:

```html
<form action="">
  <label>
    Full Name:
    <input type="text" />
  </label>
</form>
```

**Asociación explícita** — usando el atributo `for`:

```html
<form action="">
  <label for="email">Email Address: </label>
  <input type="email" id="email" />
</form>
```

> ⚠️ El valor de `for` en el label debe ser **igual** al `id` del input.

---

#### El elemento `<button>` y sus tipos

```html
<button type="button">Mostrar Formulario</button>
<button type="submit">Enviar Formulario</button>
<button type="reset">Resetear Formulario</button>
```

| Tipo | ¿Qué hace? |
|------|-----------|
| `button` | Botón genérico, no hace nada solo (necesita JavaScript) |
| `submit` | Envía el formulario |
| `reset` | Limpia todos los campos del formulario |

---

#### Los elementos `<fieldset>` y `<legend>`

- `<fieldset>` — agrupa inputs relacionados.
- `<legend>` — agrega un título/descripción al grupo.

```html
<!-- Grupo de radio buttons -->
<fieldset>
  <legend>Was this your first time at our hotel?</legend>

  <label for="yes-option">Yes</label>
  <input id="yes-option" type="radio" name="hotel-stay" value="yes" />

  <label for="no-option">No</label>
  <input id="no-option" type="radio" name="hotel-stay" value="no" />
</fieldset>

<!-- Grupo de checkboxes -->
<fieldset>
  <legend>
    Why did you choose to stay at our hotel? (Check all that apply)
  </legend>

  <label for="location">Location</label>
  <input type="checkbox" id="location" name="location" value="location" />

  <label for="price">Price</label>
  <input type="checkbox" id="price" name="price" value="price" />
</fieldset>
```

> En los **radio buttons**, darles el mismo `name` los agrupa — solo se puede seleccionar uno a la vez.

> El **focused state** es el estado del input cuando el usuario lo selecciona.

---

### Repaso de Elementos y Atributos de Tablas

#### Estructura completa de una tabla

```html
<table>
  <caption>Exam Grades</caption>

  <thead>
    <tr>
      <th>Last Name</th>
      <th>First Name</th>
      <th>Grade</th>
    </tr>
  </thead>

  <tbody>
    <tr>
      <td>Davis</td>
      <td>Alex</td>
      <td>54</td>
    </tr>

    <tr>
      <td>Doe</td>
      <td>Samantha</td>
      <td>92</td>
    </tr>

    <tr>
      <td>Rodriguez</td>
      <td>Marcus</td>
      <td>88</td>
    </tr>
  </tbody>

  <tfoot>
    <tr>
      <td colspan="2">Average Grade</td>
      <td>78</td>
    </tr>
  </tfoot>
</table>
```

**Resumen de elementos de tabla**

| Elemento | ¿Para qué sirve? |
|----------|-----------------|
| `<table>` | Contenedor principal de la tabla |
| `<thead>` | Agrupa el contenido del encabezado |
| `<tbody>` | Agrupa el contenido del cuerpo |
| `<tfoot>` | Agrupa el contenido del pie |
| `<tr>` | Crea una fila (Table Row) |
| `<th>` | Celda de encabezado (Table Header) |
| `<td>` | Celda de dato (Table Data) |
| `<caption>` | Agrega un título a la tabla |
| `colspan` | Especifica cuántas columnas debe abarcar una celda |

---

### Repaso de Herramientas HTML

| Herramienta | ¿Para qué sirve? |
|-------------|-----------------|
| **HTML Validator** | Verifica la sintaxis del HTML para asegurarse de que es válido |
| **DOM Inspector** | Permite inspeccionar y modificar la estructura HTML de una página |
| **DevTools** | Conjunto de herramientas del navegador para depurar, perfilar y analizar páginas web |

---

**Diccionario del repaso**

- Review: Repaso / Revisión.
- Span: Abarcar / Extenderse (ej. `colspan` = cuántas columnas abarca una celda).
- Focused state: Estado de enfoque (cuando un input está seleccionado por el usuario).
- Caption: Título / Leyenda (el título de una tabla).
- Group: Agrupar / Grupo (en radio buttons, los que comparten `name` forman un grupo).
- Apply: Aplicar / Seleccionar (ej. "Check all that apply" = marca todas las que apliquen).
- Related: Relacionado / Conexo.