# Informe de Auditoría Recibida

**Página revisada:** Tienda de Artesanías  
**Archivos revisados:** archivo HTML y archivo CSS  

## 1. Hallazgos de auditoría

### Hallazgo 1: Falta de CSS Grid en la estructura general
- **Requisito:** 4 – Diseño responsive
- **Ubicación:** estilos.css
- **Qué esperaba encontrar:** uso de CSS Grid para la estructura general y Flexbox para al menos un componente interno, manteniendo un diseño adaptable.
- **Hallazgo:** el archivo CSS utiliza display: flex en el menú de navegación, pero no implementa display: grid para organizar la estructura general.
- **Norma que incumple:** requisito #4 del profesor, relacionado con CSS Grid Layout.
- **Severidad:** Alta

### Hallazgo 2: Ausencia de imágenes en la página
- **Requisito:** Base 8
- **Ubicación:** index.html, contenido de la página
- **Qué esperaba encontrar:** que las imágenes informativas incluyen un alt descriptivo y que las imágenes decorativas utilicen alt="" cuando corresponda.
- **Hallazgo:** no se identificaron imágenes en el código HTML revisado. Por lo tanto, no es posible evaluar el uso del atributo alt.
- **Norma de referencia:** WCAG 2.2, criterio 1.1.1
- **Severidad:** Alta

### Hallazgo 3: Identificadores HTML con espacios
- **Requisito:** Base 7
- **Ubicación:** index.html, líneas 22 y 27
- **Qué esperaba encontrar:** identificadores id válidos, sin espacios, que permitan reconocer correctamente las secciones de la página.
- **Hallazgo:** el validador W3C detectó dos errores porque los identificadores de las secciones contienen espacios.
- **Norma que incumple:** HTML Living Standard, atributo global id.
- **Severidad:** Media

### Hallazgo 4: Valores incorrectos en el atributo scope
- **Requisito:** Base 3 – Tabla de datos y Base 7 – Validación HTML
- **Ubicación:** index.html, líneas 33, 34 y 35
- **Qué esperaba encontrar:** encabezados de tabla que utilicen correctamente scope="col".
- **Hallazgo:** el validador W3C identificó tres errores en los encabezados de la tabla debido al espacio adicional en el valor del atributo scope.
- **Norma que incumple:** HTML Living Standard, atributo scope del elemento th. Relacionado con WCAG 2.2, criterio 1.3.1 (Información y relaciones).
- **Severidad:** Media

### Hallazgo 5: Enlaces de navegación incorrectos
- **Requisito:** Base 6 – Navegación
- **Ubicación:** index.html, etiquetas <a> del menú de navegación y atributos id de las secciones
- **Qué esperaba encontrar:** que los enlaces del menú permitan desplazarse a sus secciones correspondientes.
- **Hallazgo:** los enlaces de navegación no llevan a las secciones correspondientes porque los valores de los IDs contienen espacios.
- **Norma que incumple:** requisito de navegación del profesor. HTML Living Standard (enlaces internos).
- **Severidad:** Media

## 2. Aspectos implementados correctamente

- La página contiene las etiquetas semánticas principales.
- La jerarquía de encabezados utiliza H1 y H2 correctamente.
- El formulario contiene cinco campos con sus respectivas etiquetas.
- Se utilizan los tipos date, time y email.
- El formulario incorpora required, fieldset y legend.
- El menú utiliza Flexbox.
- Los colores están definidos mediante variables CSS.

## 3. Conclusión

La página de la Tienda de Artesanías cumple varios requisitos de estructura HTML y formulario. Sin embargo, se identificaron problemas en la navegación interna, los atributos scope de la tabla y la ausencia de CSS Grid para la estructura general, también hay ausencia de imágenes y errores en los identificadores.

Se recomienda corregir los errores confirmados y completar las pruebas pendientes para garantizar el cumplimiento de los estándares web solicitados por el profesor.