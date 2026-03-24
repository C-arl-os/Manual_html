# ♿ Manual de Accesibilidad Web
_Apuntes diarios y ejemplos prácticos_

---

## 📌 Información general

| Campo | Detalle |
|------|--------|
| Autor | Carlos Sancir |
| Fecha inicio | 18/3/2026 |
| Objetivo | Aprender accesibilidad web en HTML |
| Nivel | Básico → Avanzado |

---

## 🧭 Índice

- [♿ Manual de Accesibilidad Web](#-manual-de-accesibilidad-web)
  - [📌 Información general](#-información-general)
  - [🧭 Índice](#-índice)
  - [1️⃣ Importancia de la accesibilidad y buena estructura en HTML](#1️⃣-importancia-de-la-accesibilidad-y-buena-estructura-en-html)
    - [Que es Accesibilidad?](#que-es-accesibilidad)
      - [Accesibilidad Web (Web Accessibility)](#accesibilidad-web-web-accessibility)
      - [¿Qué es la accesibilidad?](#qué-es-la-accesibilidad)
      - [Los 4 principios POUR](#los-4-principios-pour)
    - [Lectores de Pantalla (Screen Readers)](#lectores-de-pantalla-screen-readers)
      - [¿Qué son los lectores de pantalla?](#qué-son-los-lectores-de-pantalla)
      - [¿Para qué sirven?](#para-qué-sirven)
    - [Teclados de Texto Grande y Braille](#teclados-de-texto-grande-y-braille)
      - [¿Para quién son?](#para-quién-son)
      - [Teclados de Texto Grande (Large Print Keyboards)](#teclados-de-texto-grande-large-print-keyboards)
    - [Magnificadores de Pantalla (Screen Magnifiers)](#magnificadores-de-pantalla-screen-magnifiers)
      - [¿Qué son?](#qué-son)
  - [¿Cómo funcionan?](#cómo-funcionan)
  - [¿Para qué se usan?](#para-qué-se-usan)
  - [Buenas prácticas para desarrolladores](#buenas-prácticas-para-desarrolladores)
  - [Screen magnifiers integrados por sistema operativo](#screen-magnifiers-integrados-por-sistema-operativo)
  - [Magnificadores de terceros (Third-party)](#magnificadores-de-terceros-third-party)
  - [Respuestas a las preguntas de repaso](#respuestas-a-las-preguntas-de-repaso)

---

## 1️⃣ Importancia de la accesibilidad y buena estructura en HTML

### Que es Accesibilidad?

#### Accesibilidad Web (Web Accessibility)

#### ¿Qué es la accesibilidad?

La accesibilidad consiste en crear productos y servicios que **todos puedan usar**. En el contexto del desarrollo web, significa crear sitios que todos puedan entender e interactuar con ellos, incluyendo personas con discapacidades.

---

**Tipos de discapacidades que pueden afectar la experiencia web**

- Ceguera
- Visión reducida
- Daltonismo
- Sordera
- Dificultad para usar teclado, ratón o pantallas táctiles
- Trastornos de atención
- Problemas de memoria
- Dificultad para hablar o entender lenguaje hablado
- Sensibilidad a luces intermitentes

---

**¿Qué es el WCAG?**

Las **Web Content Accessibility Guidelines (WCAG)** son un conjunto de estándares internacionales desarrollados por el **W3C (World Wide Web Consortium)** para hacer los sitios web más accesibles.

> Puedes consultar la referencia completa en el sitio oficial del W3C.

---

#### Los 4 principios POUR

| Letra | Principio | ¿Qué significa? | Ejemplo |
|-------|-----------|-----------------|---------|
| **P** | Perceivable (Perceptible) | Los usuarios deben poder **percibir** la información presentada | Agregar texto alternativo (`alt`) a las imágenes para lectores de pantalla |
| **O** | Operable (Operable) | Los usuarios deben poder **interactuar** con la interfaz | Asegurarse de que todo funcione con el teclado, no solo con el ratón |
| **U** | Understandable (Comprensible) | Los usuarios deben poder **entender** la información | Usar lenguaje simple y evitar oraciones complejas |
| **R** | Robust (Robusto) | El contenido debe poder ser **interpretado** por navegadores y tecnologías de asistencia | Usar HTML semántico correcto |

> ⚠️ Si tu contenido no cumple con **alguno** de estos 4 principios, no todos podrán usar tu sitio web.

---

**¿Por qué es importante el HTML semántico para la accesibilidad?**

El HTML semántico ayuda a que los navegadores y tecnologías de asistencia (como lectores de pantalla) interpreten correctamente el contenido de tu página.

```html
<!-- ❌ No semántico - un lector de pantalla no sabe qué es esto -->
<div class="titulo">Bienvenido</div>

<!-- ✅ Semántico - el lector de pantalla sabe que es un encabezado principal -->
<h1>Bienvenido</h1>
```

---

**Resumen**

| Concepto | Descripción |
|----------|-------------|
| Accesibilidad | Crear sitios usables por todas las personas |
| W3C | Organización que desarrolla estándares web internacionales |
| WCAG | Guías para hacer sitios web accesibles |
| POUR | Los 4 principios de accesibilidad: Perceptible, Operable, Comprensible, Robusto |

---

**Respuestas a las preguntas de repaso**

1. **¿Cuál es el objetivo principal de la accesibilidad web?**
   → **Garantizar que los sitios web sean utilizables por todos.**

2. **¿Qué son las WCAG?**
   → Un **conjunto de guías para hacer los sitios web accesibles** para todos.

3. **¿Cuál de las siguientes NO es un principio central de las WCAG?**
   → **Compatible** — los 4 principios son: Perceivable, Operable, Understandable y Robust (POUR).

**Diccionary**

- Involves: Implica / Involucra.
- Disabilities: Discapacidades.
- Blindness: Ceguera.
- Low vision: Visión baja / Visión reducida.
- Color blindness: Daltonismo.
- Deafness: Sordera.
- Attention disorders: Trastornos de atención (como el TDAH).
- Flashing lights: Luces parpadeantes / Destellos (importante para evitar ataques de epilepsia).
- Guidelines: Pautas / Directrices / Guías.
- Perceivable: Perceptible (que se puede notar o percibir con los sentidos).
- Must be able: Debe ser capaz / Debe poder.
- Operable: Operable (que se puede usar o manejar, ej. con un teclado).
-  Understandable: Comprensible / Entendible.
- Robust: Robusto (que funciona bien con diferentes tecnologías y navegadores).
- Wide range: Amplia gama / Gran variedad.
- Helpful: Útil / De ayuda.
- Core: Núcleo / Esencial / Principal.
- Quick: Rápido.
- Consortium: Consorcio (como el W3C, que dicta las reglas de la web).
- Engage: Involucrarse / Participar / Interactuar.

### Lectores de Pantalla (Screen Readers)

#### ¿Qué son los lectores de pantalla?

Los **screen readers** son programas de tecnología de asistencia que ayudan a personas ciegas y con discapacidad visual a usar computadoras y dispositivos móviles.

> No son solo herramientas para ciegos — también los usan personas con dislexia y discapacidades cognitivas.

---

#### ¿Para qué sirven?

Permiten a las personas:
- Acceder a educación
- Encontrar oportunidades de trabajo
- Usar redes sociales
- Participar plenamente en la sociedad digital

---

**Funciones principales**

| Función | Descripción |
|---------|-------------|
| **Text-to-speech** | Convierte el texto en voz |
| **Braille output** | Renderiza el texto en salida braille |
| **Navigation aids** | Ayudas para navegar por la interfaz |
| **Web browsing assistance** | Asistencia para navegar sitios web |

> ⚠️ **Idea errónea común:** Mucha gente cree que los screen readers son solo dispositivos de texto a voz, pero eso es solo **una** de sus funciones.

---

**Screen readers por sistema operativo**

| Sistema Operativo | Screen Reader | Costo | Atajo para activar |
|-------------------|--------------|-------|-------------------|
| **macOS / iOS** | VoiceOver | Gratis (integrado) | `CMD + F5` (Mac) / Settings (iPhone) |
| **Windows** | Narrator | Gratis (integrado) | `WIN + CTRL + ENTER` |
| **Windows** | NVDA | Gratis (open-source) | — |
| **Windows** | JAWS | De pago | — |
| **Linux (escritorio)** | Orca | Gratis | — |
| **Linux (terminal)** | Speakup | Gratis | — |
| **Android** | TalkBack | Gratis (integrado) | Settings → Special Function → Accessibility → TalkBack |
| **Android** | Ella / Select to Speak | Gratis (algunos dispositivos) | — |

---

**¿Por qué los desarrolladores deben aprender sobre screen readers?**

Uno de los mayores desafíos para los usuarios de screen readers es que **muchos desarrolladores no diseñan sus productos pensando en accesibilidad**.

Todo desarrollador debe aprender a hacer su software accesible porque:
- Demuestra **empatía** con los usuarios
- Muestra un compromiso con la **inclusión**
- Garantiza que **todos los usuarios** puedan beneficiarse de su trabajo

---

**Resumen**

| Concepto | Descripción |
|----------|-------------|
| Screen reader | Programa que ayuda a personas ciegas/con discapacidad visual a usar dispositivos |
| Text-to-speech | Convierte texto en voz (es una función, no la definición completa) |
| VoiceOver | Screen reader integrado en macOS e iOS |
| NVDA | Screen reader gratuito y open-source para Windows |

---

**Respuestas a las preguntas de repaso**

1. **¿Cuál es el screen reader integrado en macOS e iOS?**
   → **VoiceOver**

2. **¿Para quiénes NO están hechos los screen readers?**
   → **Para personas sordas (the deaf)** — los screen readers están diseñados para discapacidades visuales y cognitivas, no auditivas.

3. **¿Cuál de estas NO es una función de los screen readers?**
   → **Speech-to-text** (voz a texto) — los screen readers convierten texto a voz, no al revés.


**Diccionary**

- Screen readers: Lectores de pantalla (software que lee el contenido de la pantalla para personas ciegas).
- Empower: Empoderar / Dar autonomía.
- Fully: Totalmente / Plenamente.
- Misconception: Idea errónea / Malentendido / Concepto equivocado.
- Text-to-speech: Texto a voz (la tecnología que convierte caracteres en audio).
- Features: Funcionalidades / Características.
- Aids: Ayudas / Herramientas de asistencia.
- Blind: Ciego/a.
- Speak up: Hablar más fuerte / Alzar la voz (también puede significar "expresarse").
- Mind: Mente (usado como "keep in mind": tener en cuenta).
- Broad topic: Tema amplio / Tema extenso.





### Teclados de Texto Grande y Braille

#### ¿Para quién son?

Los teclados de texto grande y braille están diseñados para **usuarios con discapacidades visuales**.

---

#### Teclados de Texto Grande (Large Print Keyboards)

También llamados **Large Text Keyboards**. Sus características principales son:

- Las letras, números y símbolos son **más grandes** que en un teclado estándar
- Mayor **contraste y brillo** para facilitar la lectura
- Útiles para personas con **visión reducida (low vision)**

**Ejemplos:**

| Teclado | Descripción |
|---------|-------------|
| MaxiAids (amarillo) | Teclas amarillas con letras negras, grandes y en negrita |
| Black Large Print | Teclas negras con letras blancas, además tiene **retroiluminación** ajustable |

---

**Teclados Braille**

Diseñados para personas con discapacidades visuales más severas, incluyendo personas **completamente ciegas**.

**¿Qué es el braille?**

El braille es un **sistema táctil de lectura y escritura**. Consiste en puntos elevados organizados en patrones específicos que representan letras, números y puntuación.

**¿Cómo funcionan las teclas braille?**

Las teclas tienen **puntos elevados en patrones** que representan letras, números y símbolos. El usuario los identifica **tocándolos con los dedos**.

---

**Teclados combinados**

Algunos teclados combinan **ambos enfoques**: texto grande + patrones braille en las teclas.

> Útiles tanto para personas con discapacidad visual como para personas que están **aprendiendo braille**.

---

**## Comparación de tipos de teclados**

| Tipo | ¿Para quién? | ¿Cómo ayuda? |
|------|-------------|--------------|
| Large Print | Visión reducida | Letras más grandes y mayor contraste |
| Braille | Ceguera / discapacidad visual severa | Patrones táctiles de puntos elevados |
| Combinado | Ambos grupos | Texto grande + patrones braille |

---

**Respuestas a las preguntas de repaso**

1. **¿Cuál es un beneficio de los teclados de texto grande?**
   → **Mejor legibilidad de las teclas** (Improved readability of the keys).

2. **¿Quiénes se benefician principalmente de estos teclados?**
   → **Personas con discapacidades visuales.**

3. **¿Cómo identifican las letras en un teclado braille?**
   → **Sintiendo los patrones de puntos elevados con los dedos.**

**Vocabulary**
- Helpful: Útil / De gran ayuda.
- Find: Encontrar / Hallar.
- Most of them: La mayoría de ellos/as.
- Enhanced: Mejorado / Optimizado (ej. "visibilidad mejorada").
- Brightness: Brillo.
- Bold: Negrita (en texto) / Intrépido o marcado (en diseño).
- Backlit: Retroiluminado (como los teclados que tienen luz por detrás).
- So user: "Para que el usuario..." (generalmente parte de una frase como so users can...).
- Lighting conditions: Condiciones de iluminación.
- Provide: Proporcionar / Brindar / Proveer.
- Cues: Señales / Indicaciones / Pistas (ej. visual cues son señales visuales).
- Raised dots: Puntos en relieve (característicos del sistema Braille).
- Arranged: Organizado / Dispuesto / Arreglado.
- Patterns: Patrones / Modelos.
- By feeling: Al tocar / Mediante el tacto (literalmente "sintiendo").
- Empower: Empoderar / Dar autonomía o capacidad.



---
### Magnificadores de Pantalla (Screen Magnifiers)

#### ¿Qué son?

Los **screen magnifiers** son herramientas que ayudan a personas con **visión reducida** y otras discapacidades visuales a acceder mejor al contenido digital y a la web.

---

## ¿Cómo funcionan?

Amplían textos, gráficos y otros elementos en la pantalla de una computadora o dispositivo móvil.

- Permiten ampliar la pantalla **más del 200%**
- El usuario navega usando su dispositivo de señalización o teclado
- Ofrecen **porcentajes de zoom personalizables** y otras opciones en su configuración

---

## ¿Para qué se usan?

| Uso | Descripción |
|-----|-------------|
| **Leer texto** | Amplían fuentes pequeñas en documentos o aplicaciones |
| **Navegación web** | Ayudan a localizar y hacer clic en botones, enlaces y elementos interactivos |
| **Formularios** | Permiten llenar formularios sin dificultad |
| **Contenido general** | Permiten leer emails, artículos y otro contenido sin esfuerzo visual |

---

## Buenas prácticas para desarrolladores

Para que los productos digitales sean compatibles con screen magnifiers, los desarrolladores deben:

- Usar **fuentes escalables** para que el usuario pueda redimensionar sin romper el layout
- Implementar **diseño responsivo** que se adapte a diferentes tamaños de pantalla
- Usar **esquemas de alto contraste** y colores personalizables
- Implementar una **barra de navegación pequeña y no fija** para que el contenido sea visible al usar magnificadores
- Usar **texto HTML real** en lugar de imágenes de texto
- Proporcionar **retroalimentación** directamente junto al elemento que la genera

---

## Screen magnifiers integrados por sistema operativo

| Sistema Operativo | Magnificador | Cómo activarlo |
|-------------------|-------------|----------------|
| **macOS** | Zoom | Settings → Accessibility → Zoom → activar atajos de teclado |
| **iOS (iPhone)** | Zoom | Settings → Accessibility → Zoom |
| **Android** | Magnification | Settings → Special Function → Accessibility → Magnification |
| **Windows** | Magnifier | Settings → Ease of Access → Magnifier |
| **Linux** | Zoom o Magnifier | Varía según la distribución |

---

## Magnificadores de terceros (Third-party)

| Magnificador | Sistema Operativo |
|-------------|------------------|
| **ZoomText** | Windows |
| **ClaroView** | macOS y Windows |
| **iZoom** | Windows |
| **Zoomify - Screen Magnifier** | macOS |
| **LunarPlus** | Windows |
| **Loupe** | macOS |

---

## Respuestas a las preguntas de repaso

1. **¿Cómo funcionan la mayoría de los screen magnifiers?**
   → **Ampliando los textos, gráficos y otros elementos** en la pantalla de una computadora o dispositivo móvil.

2. **¿Qué debe hacer un desarrollador para hacer sus productos compatibles con screen magnifiers?**
   → **Hacer que sus páginas respondan a diferentes tamaños de pantalla** (diseño responsivo).

3. **¿Cuál de los siguientes es un magnificador de terceros?**
   → **ZoomText**