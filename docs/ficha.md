# Ficha Personalizada - Estudiante N.º 22

## Datos de la ficha

| N.º de lista | Temática | Campos especiales del formulario | Breakpoint principal | Restricción especial |

| 22 | Tienda de artesanías | Fecha y hora de reserva | 640 px | Modo oscuro con prefers-color-scheme, sin duplicar reglas |

## Requisitos específicos de mi ficha

### Temática
- **Tienda de artesanías**: Todo el contenido de la página debe estar relacionado con una tienda de artesanías (productos, talleres, reservas, etc.)

### Campos especiales del formulario
- **Fecha y hora de reserva**: El formulario debe incluir campos específicos para fecha (`<input type="date">`) y hora (`<input type="time">`) de reserva de talleres

### Breakpoint principal
- **640 px**: El diseño responsive debe tener un breakpoint principal en 640px, donde el layout cambia significativamente entre móvil y escritorio

### Restricción especial
- **Modo oscuro con `prefers-color-scheme`, sin duplicar reglas**: 
  - Implementar modo oscuro usando la media query `prefers-color-scheme: dark`
  - NO escribir el CSS dos veces (una versión para modo claro y otra para modo oscuro)
  - Usar variables CSS (`--color-...`) y solo redefinir las variables dentro del `@media`
  - NO usar JavaScript para cambiar el tema manualmente
  - El cambio debe ser automático según la preferencia del sistema operativo del usuario

## Cumplimiento de requisitos

- [x] Temática: Tienda de artesanías
- [x] Formulario con fecha y hora de reserva
- [x] Breakpoint responsive en 640 px
- [x] Modo oscuro con `prefers-color-scheme`
- [x] Sin duplicar reglas CSS (solo variables)