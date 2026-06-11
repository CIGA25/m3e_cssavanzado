# Examen Módulo 2 - CSS Avanzado 📲

Este repositorio contiene el proyecto final correspondiente al examen del **Módulo 2** del bootcamp **Desarrollo Front-End**. El desafío consistió en consolidar e integrar de forma avanzada todos los conceptos de maquetación, responsividad y estilos dinámicos aprendidos a lo largo del módulo.

## 🔗 Revisa aquí
https://ciga25.github.io/m3e_cssavanzado/

## 🎯 Objetivos del Examen
* **Layout Avanzado con CSS Grid:** Estructurar la arquitectura global del sitio (distribución de paneles de navegación, cuerpo de contenido y pie de página) en un sistema bidimensional.
* **Componentes Flexibles (Flexbox):** Resolver de manera precisa la alineación interna, dirección y distribución espacial de los elementos dentro de los contenedores moleculares (tarjetas, barras de navegación y menús).
* **Diseño Responsivo Eficiente (Media Queries):** Garantizar la adaptabilidad y el cambio radical de comportamiento de la interfaz al transicionar de pantallas móviles a resoluciones de escritorio.
* **Animaciones:** Implementar dinámicas visuales, transiciones y animaciones personalizadas mediante CSS para enriquecer la experiencia de usuario (UI/UX).

## 🛠️ Tecnologías y Herramientas
* **HTML5 Semántico:** Estructura limpia utilizando etiquetas semánticas avanzadas (`header`, `nav`, `main`, `article`, `figure`, `footer`).
* **CSS3 Avanzado:** Uso de propiedades nativas para layouts complejos (Grid y Flexbox), selectores específicos, media queries y animaciones (`transition`, `transform`).
* **Fuentes Tipográficas (Google Fonts):** Integración de *JetBrains Mono* y *Crimson Pro* para transmitir una identidad conceptual de archivo confidencial, técnico e investigativo.
* **Iconografía:** Uso de FontAwesome para el despliegue de iconos vectoriales interactivos.

## 🌟 Implementación Técnico-Estructural Destacada

### 1. Arquitectura de Rejilla Dinámica (CSS Grid)
El cuerpo del documento utiliza el sistema de áreas de CSS Grid para alternar la disposición de sus componentes clave de manera fluida:
* **Comportamiento Base (Móvil):** El diseño se apila verticalmente en una sola columna, donde la cabecera ocupa el área superior (`lat`), seguida del contenedor principal de archivos (`main`) y cerrando con el footer (`pie`).
* **Comportamiento Tablet (@media (min-width: 768px)):** Se activa una disposición intermedia en dos columnas (`1fr 1fr`) reorganizando las filas y la distribución interna. La galería principal de archivos desclasificados (`.contenido`) aprovecha el incremento de espacio mutando a una cuadrícula simétrica de **2 columnas**.
* **Comportamiento Desktop (@media (min-width: 1024px)):** El layout experimenta un cambio estructural importante. La cabecera se transforma en un **panel lateral izquierdo fijo (Sidebar)** de ancho controlado, mientras que los archivos desclasificados y el footer se posicionan en la sección derecha, aprovechando al máximo el ancho de pantalla.

### 2. Contenedores Moleculares con Flexbox
Se aplicó el modelo de caja flexible en múltiples puntos del proyecto para lograr un control milimétrico del espacio:
* **Tarjetas de Archivos (.box-card):** Estructura que organiza verticalmente la previsualización de imágenes, metadatos tabulares de los documentos de investigación y botones de acción.
* **Navbar Móvil:** Distribución horizontal con extremos justificados (`justify-content: space-between`) para posicionar el logotipo de la organización y el menú interactivo.

### 3. Sistema Interactivos y Animaciones (UI/UX)
El portal incorpora propiedades dinámicas para crear una experiencia inmersiva:
* **Menú Hamburguesa Nativo:** Implementación sin JavaScript, resolviendo la apertura y el despliegue del menú móvil mediante la lógica de un elemento `input[type="checkbox"]` oculto conectado con un selector CSS de hermano general (`~`).
* **Transformación en tarjetas:** A las tarjetas se les aplica una leve escala, modificando su tamaño, las imagenes contenidas en ellas pasan desde un filtro gris a un full color, al hacer hover sobre ellas.
* **Transiciones en Botones:** Efectos de cambio cromático y suavizado en los estados `:hover` de las llamadas a la acción (`button`), simulando una terminal interactiva de datos.

## 📂 Estructura de Archivos del Proyecto
```
.
├── index.html          # Portal principal con la galería de archivos desclasificados ("The Lighthouse").
├── pages/
│   ├── about.html      # Sección informativa institucional (Misión, Visión y Valores de la organización).
│   └── contact.html    # Formulario de contacto estructurado para el envío de transmisiones de datos.
├── assets/
│   ├── css/
│   │   └── styles.css  # Hoja de estilos unificada (Estructuración Grid, Flexbox, Media Queries, Animaciones y tipografías).
│   └── img/            # Recursos visuales temáticos (Faro institucional e imágenes en formato `.webp` optimizadas para rendimiento web).
```

---

*Este proyecto es parte del proceso de certificación en el bootcamp de Desarrollo Front-End - 2026.*
