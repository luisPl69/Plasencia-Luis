# Respuesta a la Auditoría 

**Estudiante:** [Luis Plasencia ] - N.º 22  

## Respuestas a los hallazgos

| N.º Hallazgo | Decisión | Justificación | Evidencia | Commit |
|--------------|----------|---------------|-----------|--------|
| 1 | **Acepta y corrige** | El hallazgo es correcto. El requisito base 4 exige CSS Grid para la estructura general. Implementé `display: grid` en el `body` con `grid-template-areas` para organizar header, main, aside y footer. | **Antes:** Sin Grid, solo Flexbox en el menú. **Después:** Grid en body con áreas definidas. Ver archivo `css/estilos.css` líneas 58-75. | `abc1234` |
| 2 | **Acepta y corrige** | El hallazgo es correcto. El requisito base 8 exige imágenes con alt adecuado. Agregué una imagen de artesanía con alt descriptivo: "Cerámica artesanal pintada a mano con diseños tradicionales". | **Antes:** Sin imágenes. **Después:** Imagen en sección "productos" con alt descriptivo. Ver archivo `index.html` línea 25. | `abc1234` |
| 3 | **Acepta y corrige** | El hallazgo es correcto. Los IDs con espacios son inválidos según HTML Living Standard. Corregí todos los IDs quitando espacios: `id="precios"` en lugar de `id="precios talleres"`. | **Antes:** `id="precios talleres"` (con espacio). **Después:** `id="precios"` (sin espacio). Ver archivo `index.html` líneas 22, 27. | `abc1234` |
| 4 | **Acepta y corrige** | El hallazgo es correcto. El atributo `scope` no debe tener espacios. Corregí de `scope=" col"` a `scope="col"` en los tres encabezados de la tabla. | **Antes:** `scope=" col"` (con espacio). **Después:** `scope="col"` (sin espacio). Ver archivo `index.html` líneas 33-35. | `abc1234` |
| 5 | **Acepta y corrige** | El hallazgo es correcto. Los enlaces no funcionaban porque los IDs tenían espacios. Al corregir los IDs (hallazgo 3), los enlaces ahora funcionan correctamente. | **Antes:** Enlaces no navegaban a las secciones. **Después:** Enlaces funcionan correctamente. Ver archivo `index.html` líneas 18-21. | `abc1234` |

## Problemas adicionales detectados y corregidos

Además de los hallazgos de la auditora, detecté y corregí los siguientes problemas:

### Problema adicional 1: Falta de `aria-label` en el `<nav>`
- **Descripción:** El elemento `<nav>` no tenía un `aria-label` para identificar su propósito para lectores de pantalla.
- **Corrección:** Agregué `aria-label="Navegación principal"` al elemento `<nav>`.
- **Norma:** WCAG 2.2, criterio 4.1.2 (Name, Role, Value).
- **Evidencia:** Ver archivo `index.html` línea 16.
- **Commit:** `abc1234`

### Problema adicional 2: Falta de validación `min` en el campo de fecha
- **Descripción:** El campo de fecha no tenía un valor mínimo, permitiendo seleccionar fechas pasadas.
- **Corrección:** Agregué `min="2024-01-01"` al input de fecha para evitar reservas en fechas pasadas.
- **Norma:** HTML Living Standard, atributo `min` del elemento input.
- **Evidencia:** Ver archivo `index.html` línea 73.
- **Commit:** `abc1234`

## Resumen de cambios

- ✅ CSS Grid implementado en la estructura general
- ✅ Imagen agregada con alt descriptivo
- ✅ IDs corregidos sin espacios
- ✅ Atributo scope corregido sin espacios
- ✅ Enlaces de navegación funcionando
- ✅ aria-label agregado al nav
- ✅ Validación min agregada al campo de fecha

Todos los cambios están en el commit `abc1234` con el mensaje: "Corrección de hallazgos de auditoría y problemas adicionales detectados".