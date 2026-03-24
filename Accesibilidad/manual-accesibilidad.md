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
    - [Software de Reconocimiento de Voz (Voice Recognition Software)](#software-de-reconocimiento-de-voz-voice-recognition-software)
      - [¿Qué es?](#qué-es)
      - [¿Para qué se usa?](#para-qué-se-usa)
- [Herramientas de Auditoría de Accesibilidad](#herramientas-de-auditoría-de-accesibilidad)
  - [¿Qué es una herramienta de auditoría de accesibilidad?](#qué-es-una-herramienta-de-auditoría-de-accesibilidad)
  - [Herramientas gratuitas de auditoría](#herramientas-gratuitas-de-auditoría)
    - [1. Google Lighthouse](#1-google-lighthouse)
    - [2. WAVE](#2-wave)
    - [3. IBM Equal Access Accessibility Checker](#3-ibm-equal-access-accessibility-checker)
  - [Comparación de herramientas](#comparación-de-herramientas)
  - [Recuerda siempre](#recuerda-siempre)
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

#### ¿Cómo funcionan?

Amplían textos, gráficos y otros elementos en la pantalla de una computadora o dispositivo móvil.

- Permiten ampliar la pantalla **más del 200%**
- El usuario navega usando su dispositivo de señalización o teclado
- Ofrecen **porcentajes de zoom personalizables** y otras opciones en su configuración

---

#### ¿Para qué se usan?

| Uso | Descripción |
|-----|-------------|
| **Leer texto** | Amplían fuentes pequeñas en documentos o aplicaciones |
| **Navegación web** | Ayudan a localizar y hacer clic en botones, enlaces y elementos interactivos |
| **Formularios** | Permiten llenar formularios sin dificultad |
| **Contenido general** | Permiten leer emails, artículos y otro contenido sin esfuerzo visual |

---

**Buenas prácticas para desarrolladores**

Para que los productos digitales sean compatibles con screen magnifiers, los desarrolladores deben:

- Usar **fuentes escalables** para que el usuario pueda redimensionar sin romper el layout
- Implementar **diseño responsivo** que se adapte a diferentes tamaños de pantalla
- Usar **esquemas de alto contraste** y colores personalizables
- Implementar una **barra de navegación pequeña y no fija** para que el contenido sea visible al usar magnificadores
- Usar **texto HTML real** en lugar de imágenes de texto
- Proporcionar **retroalimentación** directamente junto al elemento que la genera

---

**Screen magnifiers integrados por sistema operativo**

| Sistema Operativo | Magnificador | Cómo activarlo |
|-------------------|-------------|----------------|
| **macOS** | Zoom | Settings → Accessibility → Zoom → activar atajos de teclado |
| **iOS (iPhone)** | Zoom | Settings → Accessibility → Zoom |
| **Android** | Magnification | Settings → Special Function → Accessibility → Magnification |
| **Windows** | Magnifier | Settings → Ease of Access → Magnifier |
| **Linux** | Zoom o Magnifier | Varía según la distribución |

---

**Magnificadores de terceros (Third-party)**

| Magnificador | Sistema Operativo |
|-------------|------------------|
| **ZoomText** | Windows |
| **ClaroView** | macOS y Windows |
| **iZoom** | Windows |
| **Zoomify - Screen Magnifier** | macOS |
| **LunarPlus** | Windows |
| **Loupe** | macOS |

---

**Respuestas a las preguntas de repaso**

1. **¿Cómo funcionan la mayoría de los screen magnifiers?**
   → **Ampliando los textos, gráficos y otros elementos** en la pantalla de una computadora o dispositivo móvil.

2. **¿Qué debe hacer un desarrollador para hacer sus productos compatibles con screen magnifiers?**
   → **Hacer que sus páginas respondan a diferentes tamaños de pantalla** (diseño responsivo).

3. **¿Cuál de los siguientes es un magnificador de terceros?**
   → **ZoomText**

**Diccionary**
- Magnifiers: Lupas / Amplificadores (se refiere tanto al objeto físico como al software de lupa en Windows/macOS).
- Impairments: Discapacidades / Deficiencias / Deterioros (ej. visual impairments).
- Let's delve deeper into: Profundicemos en / Indaguemos más a fondo en.
- Enlarging: Agrandar / Ampliar.
- Features: Funciones / Características.
- By enlarging: Al agrandar / Mediante la ampliación.
- Staining: Esfuerzo / Fatiga (en contexto de vista: eye straining). También puede significar "manchar" en otros contextos.
- Fill out forms: Rellenar formularios / Completar formularios.
- Engage: Interactuar / Participar / Involucrarse.
- Mainstay: Pilar / Sustento principal / Elemento básico.
- By going: Al ir / Yendo.
- Toggle: Alternar / Conmutar (el botón o acción de activar/desactivar algo).
- May vary from: Puede variar de / Puede ser diferente según.
---

### Software de Reconocimiento de Voz (Voice Recognition Software)

#### ¿Qué es?

El **software de reconocimiento de voz** ayuda a personas con discapacidades a interactuar con computadoras y dispositivos digitales usando su **voz** en lugar de dispositivos de entrada tradicionales como teclados y ratones.

---

#### ¿Para qué se usa?

Permite a los usuarios con discapacidades:

- Escribir emails y otros documentos
- Navegar por internet
- Controlar dispositivos de hogar inteligente (smart home)
- Ejecutar comandos en la computadora

> Al eliminar la necesidad de interacción física, el software de reconocimiento de voz otorga **independencia y control** a las personas con discapacidades.

---

**¿Quiénes se benefician?**

| Grupo | Razón |
|-------|-------|
| Personas con discapacidades visuales | Ceguera o visión reducida |
| Personas con discapacidades de movilidad | Uso limitado de manos y brazos, artritis, síndrome del túnel carpiano |
| Personas en recuperación | Lesiones en manos o brazos |
| Personas con trastornos cognitivos | Problemas de memoria o trastorno de déficit de atención |
| Personas mayores | Pueden encontrar más fácil usar comandos de voz |

> 💡 Las personas con discapacidades **no son las únicas** que usan esta tecnología. También la usan fuerzas del orden, gamers, conductores y profesionales ocupados.

---

**Software de reconocimiento de voz por plataforma**

| Software | Plataforma | Tipo |
|----------|-----------|------|
| **Voice Control** | macOS / iOS | Integrado |
| **Voice Access** | Android / Windows (versiones recientes) | Integrado |
| **Windows Speech Recognition** | Windows | Integrado |
| **Dragon by Nuance** | Windows | Terceros (popular) |

---

**Comparación: Dispositivos tradicionales vs Voz**

| | Teclado y ratón | Reconocimiento de voz |
|---|---|---|
| Requiere movimiento físico | ✅ Sí | ❌ No |
| Accesible para movilidad limitada | ❌ Difícil | ✅ Sí |
| Accesible para visión reducida | ❌ Difícil | ✅ Sí |
| Velocidad para usuarios experimentados | ✅ Alta | ✅ Alta |

---

**Respuestas a las preguntas de repaso**

1. **¿Qué dispositivos de entrada reemplaza el software de reconocimiento de voz?**
   → **Teclados y ratones** (keyboards and mice).

2. **¿Quién sería el menos beneficiado por el software de reconocimiento de voz?**
   → **Personas con poco movimiento en las piernas** — el reconocimiento de voz ayuda con limitaciones de manos, brazos y visión, no de piernas.

3. **¿Cuál de los siguientes NO es un software de reconocimiento de voz?**
   → **Audacity** — es un editor de audio, no un software de reconocimiento de voz.

**Dictionary**

- Disabilities: Discapacidades.
- Interact: Interactuar.
- Let's: Vamos a... / Hagamos... (contracción de let us, usada para proponer una acción).
- Instead: En su lugar / En vez de eso.
- Input: Entrada / Entrada de datos (ej. keyboard input es la entrada por teclado).
- Surfing: Navegar (específicamente "navegar por la red").
- Net: Red / Internet (forma corta de The Internet).
- Impairments: Deficiencias / Deterioros / Discapacidades.
- Carpal tunnel: Túnel carpiano (la zona de la muñeca que suele inflamarse por el uso repetitivo del mouse).
- Arm injuries: Lesiones en el brazo.
- Law: Ley.
- Enforcement: Aplicación / Ejecución / Cumplimiento (ej. law enforcement se traduce como "fuerzas del orden" o "aplicación de la ley").


---
# Herramientas de Auditoría de Accesibilidad

## ¿Qué es una herramienta de auditoría de accesibilidad?

Es una aplicación que ayuda a **mejorar la accesibilidad** del contenido digital reportando problemas que pueden encontrarse mediante pruebas automatizadas. Aplica para sitios web, aplicaciones web y apps móviles.

> ⚠️ **Limitación importante:** Las herramientas automatizadas solo detectan aproximadamente **un tercio** de todos los posibles problemas de accesibilidad. Siempre se requieren **pruebas manuales**, preferiblemente realizadas por personas con discapacidades.

---

## Herramientas gratuitas de auditoría

### 1. Google Lighthouse

Herramienta popular de métricas web. Se puede usar directamente en **Chrome DevTools** o en línea.

**Métricas que evalúa:**
- Accesibilidad
- SEO
- Mejores prácticas
- Rendimiento

**¿Cómo usarlo en DevTools?**
1. Abre DevTools con `F12`
2. Ve a la pestaña **Lighthouse**
3. Selecciona las métricas que quieres revisar
4. Elige el dispositivo a simular
5. Haz clic en **"Analyze page load"**
6. Revisa el puntaje y la lista de problemas

**Versión web:** `pagespeed.web.dev`

| Versión | ¿Soporta sitios locales? |
|---------|--------------------------|
| DevTools (Chrome) | ✅ Sí |
| Web (pagespeed.web.dev) | ❌ No |

---

### 2. WAVE

Herramienta confiable de accesibilidad disponible como **extensión de Chrome** o en la web.

**¿Cómo usarlo?**
- Ingresa la URL de tu sitio web
- Se genera automáticamente un reporte completo que incluye:
  - Funcionalidades de accesibilidad implementadas
  - ARIA
  - Contraste de colores

---

### 3. IBM Equal Access Accessibility Checker

Herramienta robusta para mejorar la accesibilidad del contenido digital. Disponible como **extensión de Chrome** o **add-on de Firefox**.

**¿Cómo usarlo como extensión de Chrome?**
1. Descárgala desde la Chrome Web Store
2. Abre DevTools con `F12`
3. Ve a la pestaña **"Accessibility Checker"** en el panel Elements
4. Haz clic en el botón **Scan**
5. Revisa el reporte generado
6. Exporta el reporte con **"Export XLS"** (formato Excel y HTML)

---

## Comparación de herramientas

| Herramienta | Disponible como | ¿Sitios locales? |
|-------------|----------------|-----------------|
| **Google Lighthouse** | DevTools / Web | ✅ Solo en DevTools |
| **WAVE** | Extensión Chrome / Web | ❌ No |
| **IBM Equal Access** | Extensión Chrome / Add-on Firefox | ✅ Sí |

---

## Recuerda siempre

Las herramientas automatizadas son un **punto de partida**, no una solución completa:

- Un puntaje perfecto **no significa** que tu contenido sea 100% accesible
- El rango de problemas que detectan es **limitado**
- Siempre se necesitan **pruebas manuales** para garantizar una experiencia más accesible

---

## Respuestas a las preguntas de repaso

1. **¿Cuál describe mejor una herramienta de auditoría de accesibilidad?**
   → **Evalúa qué tan accesible es tu contenido digital.**

2. **¿Cómo se puede usar el IBM Equal Access Accessibility Checker?**
   → **Como extensión de Chrome, add-on de Firefox, o paquete NPM.**

3. **¿Cuál es una limitación de la versión web de Google Lighthouse?**
   → **No puede probar sitios web locales.**