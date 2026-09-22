# Taller Integrador Individual Cortes 1 y 2

**Desarrollador:** Samuel David Ordoñez Sinisterra

## Tabla de hallazgos de la auditoría

| Defecto encontrado | Por qué era un problema | Cómo lo corrigió |
| :--- | :--- | :--- |
| Nombres de archivos con espacios y mayúsculas (`Mi Pagina De Notas_2.HTML`, `Estilos Del Sitio_2.CSS`) | Rompe las convenciones de nomenclatura web. Puede causar errores de rutas al desplegar en diferentes sistemas operativos o servidores. | Se renombraron a `index.html` y `styles.css` aplicando kebab-case. |
| Título genérico `<title>pagina</title>` | No aporta información al usuario ni a los motores de búsqueda sobre el propósito real del sitio en la pestaña del navegador. | Se cambió a `<title>Calculadora de Promedio</title>`. |
| Clase CSS no semántica (`.cont1`) | El nombre no describe la función estructural del contenedor, dificultando el mantenimiento y legibilidad del estilo. | Se renombró a `.contenedor-calculadora`. |
| IDs de elementos HTML no descriptivos (`n1`, `n2`, `n3`, `r`, `r2`) | Los identificadores cortos obligan al programador a deducir qué elemento del DOM representan o qué dato capturan. | Se cambiaron a nombres claros: `nota1`, `nota2`, `nota3`, `resultadoPromedio`, `estadoAprobacion`. |
| Nombres de variables de una letra (`a`, `b`, `c`, `x`) | No indican qué dato almacenan. `x` actúa como un número mágico, lo que dificulta la lectura y comprensión de la lógica. | Se renombraron a `valorNota1`, `valorNota2`, `valorNota3` y se creó `const cantidadNotas = 3`. |
| Convención de nombres incorrecta (`TempValue2`) | Usa PascalCase, lo cual se reserva para clases, en lugar de camelCase para variables. Además, su nombre no es semántico. | Se cambió a `let promedioCalculado`. |
| Nombre de función abreviado y ambiguo (`calc()`) | No expresa claramente la acción específica que realiza el bloque de código, limitando su entendibilidad. | Se modificó a `calcularPromedio()`. |
| Código muerto y variables sin uso (`let data1 = [];` y función `calcularAntiguo`) | Aumentan el peso del archivo innecesariamente, generan ruido visual y confusión para otros desarrolladores que lean el código. | Se eliminaron completamente del documento. |

## Enlace al sitio publicado
