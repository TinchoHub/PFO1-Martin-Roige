# PFO1: Landing Page de Portafolio Personal — Martin Roige

Este repositorio contiene el código fuente y la documentación técnica de la **Práctica Formativa Obligatoria 1 (PFO1)**
Se trata de una landing page de portafolio profesional desarrollada íntegramente con **HTML5 semántico** y **CSS3 puro**, sin frameworks externos y optimizada bajo estándares de accesibilidad (a11y), responsive design y alto rendimiento.

---

## 🔗 Enlaces del Proyecto

* **Repositorio en GitHub:** [https://github.com/TinchoHub](https://github.com/TinchoHub)[cite: 1]
* **Despliegue en Vercel:** [https://pfo-1-martin-roige.vercel.app](https://pfo-1-martin-roige.vercel.app) 

---

## 🛠️ Tecnologías y Requisitos Técnicos Cumplidos

### 1. Estructura y Semántica HTML5
- **Estructura jerárquica estricta:** Implementación de las etiquetas estructurales principales `<header>`, `<nav>`, `<main>`, `<section>`, `<article>` y `<footer>`.
- **Accesibilidad web (a11y):** Roles ARIA integrados (`role="banner"`, `role="menubar"`, `role="contentinfo"`, atributos `aria-label` y `aria-hidden`), salto de contenido (`.sr-only focus-skip`) para navegación por teclado, y etiquetas `<label>` estrictamente vinculadas mediante `for`/`id` en todos los controles del formulario.
- **4 Comentarios explicativos:** Documentación interna dentro del código `index.html` explicando las decisiones estructurales más relevantes.
- **Datos Estructurados:** Bloque `application/ld+json` con esquema `Person` para indexación semántica SEO.

### 2. Maquetación y Layout: Grid + Flexbox
- **Uso combinado y justificado:**
  - **CSS Grid:** Se utiliza en la maquetación bidimensional fluida de las secciones de **Habilidades**, **Proyectos**, **Intereses** y la grilla asimétrica de 2 columnas en **Sobre mí**. Garantiza auto-adaptación con `repeat(auto-fit, minmax(...))` evitando saltos abruptos.
  - **Flexbox:** Se emplea en componentes unidimensionales como la barra de navegación (`.nav-container`), el alineado de botones de acción, las listas de insignias/tags y el pie de página (`.footer-container`).
- **Unidades relativas y diseño fluido:** Uso integral de funciones matemáticas modernas (`clamp()`, `rem`, `%`, `vh`) para tipografía y espaciados.

### 3. Estilización y Google Fonts
- **Variables CSS (`:root`):** Paleta oscura profesional basada en escalas Ink (`#0d0f14`), acentos en Cyan/Brand (`#0a9fdc`, `#33bcf5`) y toques de contraste Gold (`#edb200`).
- **Tipografías:** Integración de *Space Grotesk* (títulos técnicos y badges) e *Inter* (lectura óptima en párrafos y cuerpos).

### 4. Interactividad, Transiciones y Animaciones
- **Animaciones personalizadas con `@keyframes`:** Entrada suave `fadeUp` en el Hero, resplandor palpitante `pulseRing` en el estado de disponibilidad y cursor de terminal `blink`.
- **Transiciones fluidas (`card-glow`):** Microinteracciones en `:hover` y `:focus-within` en todas las tarjetas de proyectos y habilidades con elevación en eje Y y sombreados reactivos.
- **Menú Móvil Nativo:** Funcionamiento 100% responsivo sin JavaScript mediante la técnica `:checked` en inputs CSS.

---

## 🎨 Secciones del Portafolio

1. **Hero Section:** Presentación personal, badge de estado, botones CTA hacia contacto y GitHub, estadísticas clave y widget interactivo de simulación de terminal.
2. **Sobre Mí:** Resumen de perfil profesional, tarjeta flotante *Clean Code* y métricas de valor *Full cycle*.
3. **Habilidades Técnicas:** Tarjetas organizadas por Frontend, Backend & APIs, y Bases de Datos / Tools.
4. **Proyectos Seleccionados:** Tarjetas con enlaces directos a repositorios (Optimizador de rutas, Panel de gestión .NET, Monitor IoT).
5. **Intereses & Proyección (Sección personal a elección):** Logística de última milla, Automatización IoT y Lógica de videojuegos RPG.
6. **Contacto:** Formulario completo con validaciones nativas y enlaces a redes.

---

## 🤖 Declaración de Uso de Inteligencia Artificial (Requisito Transversal)

En cumplimiento de las pautas de honestidad académica y autoría transparente, se detalla el uso de herramientas generativas durante el proyecto:

### 1. Herramientas utilizadas y propósito
- **Herramienta:** Asistente de IA (Gemini / Claude).
- **Propósito:** Generación de la estructura base HTML5 accesible, ayuda en la configuración de la sintaxis de variables CSS y refactorización para desacoplar clases de frameworks hacia CSS puro modular.

### 2. Tipo de suscripción
- **Plan:** Versión estándar / gratuita.

### 3. Experiencia previa
- Familiaridad intermedia en el uso de modelos de lenguaje para resolver consultas de sintaxis web y optimización de código.

### 4. Adaptación y cambios realizados con criterio propio
- **Depuración de dependencias y código generado:** Se eliminaron etiquetas propietarias de frameworks (`data-tsd-source`) y clases sobredimensionadas de Tailwind/CSS-in-JS, transformándolas en reglas semánticas y legibles en `styles.css`.
- **Accesibilidad y Rúbrica:** Se añadieron manualmente los 4 comentarios explicativos requeridos por la rúbrica, se estructuraron las etiquetas `<label>` con sus inputs en el formulario y se configuraron los roles ARIA en la barra de navegación y el footer.
- **Unificación de componentes:** Se integraron las tarjetas de la sección *Proyectos* preservando la estética oscura y los efectos visuales *glow* para una coherencia gráfica total.
