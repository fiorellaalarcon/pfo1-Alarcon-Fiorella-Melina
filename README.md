# Portafolio Personal PFO1 — Fiorella Melina Alarcón
---------------------------------------------------------
IFTS 29 - Tecnicatura Superior en Desarrollo de Software.
Agosto 2026
Desarrollo de Sistemas Web (Front End) - 2° A
Docente: Luciano Martínez.
---------------------------------------------------------

Landing page de portafolio personal desarrollada para la **PFO1**, utilizando **HTML5 y CSS3 puro**, sin frameworks.

El objetivo del proyecto es presentar mi perfil como desarrolladora de software, mostrar mis habilidades técnicas, explicar mi enfoque profesional y proporcionar una vía de contacto, aplicando buenas prácticas de desarrollo web, accesibilidad, diseño responsive y organización semántica.

**🔗 Perfil de GitHub:** https://github.com/fiorellaalarcon

**🔗 URL de Vercel:** https://pfo1-alarcon-fiorella-melina.vercel.app/

**🔗 URL del repositorio PFO1:** https://github.com/fiorellaalarcon/pfo1-alarcon-fiorella-melina

---

## 1. Descripción de la PFO1

La consigna propone desarrollar una landing page de portafolio personal utilizando HTML y CSS.

La página presenta:

* Nombre y apellido.
* Perfil como desarrolladora de software.
* Fotografía personal.
* Presentación profesional.
* Habilidades técnicas.
* Sección personal de enfoque profesional.
* Formulario de contacto.
* Enlace visible y funcional al perfil de GitHub.
* Diseño responsive.
* Animaciones y transiciones.
* HTML5 semántico.
* Buenas prácticas de accesibilidad.

Para la identidad visual elegí un enfoque **Cyber-Dark**, inspirado en interfaces de desarrollo de software y terminales modernas.

La combinación principal utiliza:

* Fondo oscuro: `#0d1117`
* Superficies oscuras con matiz púrpura.
* Fucsia neón: `#ff007f`
* Fucsia claro: `#ff3399`
* Texto blanco: `#ffffff`
* Texto secundario gris: `#9da4ae`

El fucsia funciona como color principal de identidad visual, utilizándose en botones, enlaces, bordes, indicadores, títulos y efectos de iluminación.

---

## 2. Estructura del proyecto

```text
├── index.html
├── style.css
├── logo.jpg
└── README.md
```

### `index.html`

Contiene toda la estructura semántica de la landing:

* `header`
* `nav`
* `main`
* `section`
* `article`
* `aside`
* `form`
* `footer`

### `style.css`

Contiene todo el sistema visual del proyecto:

* Variables CSS.
* Tipografías.
* Responsive design.
* Flexbox.
* CSS Grid.
* Animaciones.
* Transiciones.
* Estados hover y focus.
* Estética Cyber-Dark.
* Efectos de iluminación fucsia.

### `logo.jpg`

Imagen utilizada como fotografía principal del perfil y como pequeño elemento visual de identificación en el encabezado.

---

## 3. Decisiones de diseño

### Estética Cyber-Dark

Elegí una estética oscura con predominancia de fucsia neón porque permite representar visualmente un perfil relacionado con el desarrollo de software.

El fondo oscuro genera contraste con el contenido y permite que el fucsia funcione como elemento de identidad visual.

También incorporé:

* Cuadrícula tecnológica de fondo.
* Líneas y bordes fucsia.
* Ventana de código simulada.
* Tipografía monoespaciada.
* Efectos de glow.
* Tarjetas con interacción hover.

La intención es representar visualmente la relación entre código, tecnología y organización de información.

---

## 4. HTML5 semántico y accesibilidad

La estructura utiliza elementos semánticos de HTML5 para organizar correctamente el contenido.

Se utilizaron:

* `<header>` para la cabecera.
* `<nav>` para la navegación principal.
* `<main>` para el contenido central.
* `<section>` para las diferentes áreas del portafolio.
* `<article>` para las tarjetas de habilidades.
* `<aside>` para información complementaria.
* `<form>` para el contacto.
* `<footer>` para la información final.

También se incorporaron recursos de accesibilidad:

* Texto alternativo mediante `alt` en imágenes.
* `aria-label` para enlaces y navegación.
* `aria-labelledby` para relacionar secciones con sus encabezados.
* `aria-current="page"` en el enlace activo.
* Enlace `skip-link` para navegación mediante teclado.
* Estados `:focus-visible`.
* Etiquetas `<label>` correctamente relacionadas con los campos del formulario.
* Atributos `autocomplete`.
* Soporte para `prefers-reduced-motion`.

---

## 5. Flexbox y CSS Grid

Se utilizaron ambas tecnologías de maquetación de manera intencional.

### CSS Grid

Se utiliza principalmente en:

* Grilla de habilidades.
* Sección "Sobre mí".
* Sección de enfoque profesional.

En la grilla de habilidades se utiliza:

```css
grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
```

Esta solución permite que las tarjetas se adapten automáticamente al ancho disponible.

### Flexbox

Se utiliza principalmente en:

* Header.
* Navegación.
* Hero.
* Botones.
* Formularios.
* Footer.
* Elementos internos de las tarjetas.

Flexbox resulta apropiado en estos casos porque se trata principalmente de distribuciones unidimensionales.

La combinación de ambas tecnologías permite construir una interfaz flexible y responsive sin depender de frameworks.

---

## 6. Sistema de diseño mediante variables CSS

La paleta y las características principales de la interfaz están centralizadas mediante variables CSS dentro de `:root`.

Por ejemplo:

```css
:root {
    --bg-main: #0d1117;
    --primary: #ff007f;
    --text-main: #f0f6fc;
}
```

Esto facilita mantener la coherencia visual y modificar posteriormente la identidad de la página desde un único lugar.

---

## 7. Tipografías

Se utilizaron Google Fonts para diferenciar los roles visuales:

* **Montserrat:** títulos principales y encabezados.
* **Open Sans:** textos y contenido general.
* **Fira Code:** navegación, etiquetas y elementos que representan código.

La combinación busca equilibrar legibilidad con una estética tecnológica.

---

## 8. Animaciones y transiciones

La página incorpora animaciones personalizadas mediante `@keyframes`.

### `fadeInUp`

Se utiliza para la aparición progresiva del contenido principal.

### `pulseGlow`

Se utiliza para generar un resplandor pulsante en el botón principal.

### `statusPulse`

Anima el indicador de disponibilidad del perfil.

### `gridMove`

Anima suavemente la cuadrícula tecnológica del Hero.

### `floatingCode`

Produce un movimiento vertical sutil en el elemento visual de la sección de enfoque profesional.

Además, se utilizan transiciones en:

* Botones.
* Tarjetas.
* Imagen de perfil.
* Logo.
* Campos del formulario.
* Enlaces de navegación.

También se incorporó:

```css
@media (prefers-reduced-motion: reduce)
```

para reducir las animaciones cuando el usuario tiene configurada esa preferencia de accesibilidad.

---

## 9. Responsive Design

El sitio fue desarrollado utilizando unidades relativas, `clamp()`, CSS Grid, Flexbox y media queries.

Se contemplan diferentes tamaños de pantalla:

* Escritorio.
* Tablet.
* Smartphone.
* Pantallas pequeñas.

La grilla de habilidades utiliza `auto-fit` y `minmax()` para adaptar automáticamente la cantidad de columnas disponibles.

---

## 10. GitHub

El perfil de GitHub está enlazado de forma visible desde:

* Botón principal del Hero.
* Footer.

Perfil:

https://github.com/fiorellaalarcon

---

## 11. Publicación en Vercel

El proyecto será publicado utilizando Vercel.

**URL del proyecto:** completar una vez realizada la publicación.

La entrega final debe realizarse mediante el enlace al repositorio público correspondiente.

---

## 12. Uso de imágenes

La imagen `logo.jpg` corresponde a la imagen utilizada para representar el perfil dentro de la landing.

Imagen generada con Gemini Nano Banana Pro (versión gratuita) y editada manualmente con Microsoft Paint.
`logo.png`. Fue seleccionada y refinada mediante procesos de edición digital y diseño gráfico tradicional para garantizar los estándares de calidad del proyecto.

---

## 13. Declaración de uso de Inteligencia Artificial

Durante el desarrollo de la PFO1 utilicé **ChatGPT**, de OpenAI, como herramienta de asistencia para revisar y mejorar el código HTML5, CSS3 y la documentación del proyecto. Gemini Nano Banana Pro para la primera versión del logo.

**Herramienta utilizada:** ChatGPT — GPT-5.6 Luna.

**Plan utilizado:**  Gratuito.

### ¿Para qué utilicé IA?

La herramienta fue utilizada principalmente para:

* Revisar la estructura HTML5.
* Comparar el código con los requisitos de la consigna.
* Detectar posibles problemas de semántica.
* Revisar aspectos de accesibilidad.
* Proponer mejoras de organización del CSS.
* Revisar el uso de Flexbox y CSS Grid.
* Proponer mejoras responsive.
* Diseñar y ajustar animaciones mediante `@keyframes`.
* Mejorar la coherencia visual del sistema Cyber-Dark.
* Revisar y reorganizar la documentación del README.
* Sugerir mejoras para alcanzar los criterios superiores de la rúbrica.

La IA fue utilizada como herramienta de apoyo y no como sustituto de la toma de decisiones durante el desarrollo.

### Experiencia previa

Ya tenía experiencia previa utilizando herramientas de inteligencia artificial como apoyo para tareas relacionadas con código, redacción, revisión y resolución de errores.

La utilicé principalmente como herramienta de consulta para detectar problemas que podían pasar inadvertidos durante la revisión manual.

### Qué revisé, cambié y adapté con criterio propio

Después de recibir sugerencias de la herramienta, revisé manualmente las modificaciones antes de incorporarlas al proyecto.

Entre las decisiones tomadas y adaptadas se encuentran:

* Selección de la estética Cyber-Dark.
* Elección del fucsia `#ff007f` como color principal.
* Definición de la estructura general de la landing.
* Selección y organización de las secciones.
* Selección de la fotografía utilizada.
* Redacción y adaptación del contenido personal.
* Selección de las habilidades que aparecen en la página.
* Distribución de los elementos mediante Grid y Flexbox.
* Elección de las animaciones.
* Ajustes de accesibilidad.
* Adaptación del diseño para dispositivos móviles.
* Revisión de los textos y de la presentación visual.

La versión final fue revisada y adaptada para que el resultado responda específicamente a la consigna de la PFO1 y a las decisiones personales de diseño.

---

## 14. Ejecución local

El proyecto no requiere instalación de dependencias.

Para ejecutarlo localmente se puede:

1. Descargar o clonar el repositorio.
2. Abrir `index.html` directamente en un navegador.
3. O utilizar una extensión como Live Server desde Visual Studio Code.

No se utilizan frameworks ni librerías JavaScript externas.

---

## 15. Checklist de la consigna

* [x] HTML5 semántico.
* [x] `DOCTYPE` correcto.
* [x] `header`.
* [x] `nav`.
* [x] `main`.
* [x] `footer`.
* [x] Metaetiquetas.
* [x] CSS propio.
* [x] Google Fonts.
* [x] Flexbox.
* [x] CSS Grid.
* [x] Diseño responsive.
* [x] Animaciones personalizadas.
* [x] Transiciones.
* [x] `@keyframes`.
* [x] Imágenes con `alt`.
* [x] Formulario con `label`.
* [x] Accesibilidad mediante teclado.
* [x] `aria-label` y `aria-labelledby`.
* [x] Enlace visible a GitHub. https://github.com/fiorellaalarcon
* [x] Sección personal.
* [x] README.
* [x] Declaración de uso de IA.
* [x] URL de Vercel. https://pfo1-alarcon-fiorella-melina.vercel.app/
* [x] URL definitiva del repositorio. https://github.com/fiorellaalarcon/pfo1-alarcon-fiorella-melina

---

## 16. Conclusión

La PFO1 busca representar mi perfil profesional mediante una landing page que combine desarrollo web, organización de información y una identidad visual tecnológica.

El diseño Cyber-Dark con predominancia de fucsia fue elegido para diferenciar visualmente el portafolio y reforzar su relación con el desarrollo de software, mientras que el uso de HTML5 semántico, CSS Grid, Flexbox, responsive design y recursos de accesibilidad permite mantener una estructura técnicamente sólida.
