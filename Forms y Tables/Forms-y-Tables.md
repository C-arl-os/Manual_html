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