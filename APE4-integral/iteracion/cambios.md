# Registro de cambios · prototipo CaféU

## v3 (construcción · APE 4 integral)

| Código | Cambio | Problema que corrige | Archivo |
|---|---|---|---|
| D1 | Mensaje de pago rechazado aclara que no hubo cobro y que el pedido sigue guardado. | D1 · Alta | `prototipo/v3/index.html` |
| D2 | Búsqueda sin distinguir tildes ni mayúsculas, también por descripción. | D2 · Alta | `prototipo/v3/index.html` |
| D3 | «−» con cantidad 1 propone eliminar con confirmación. | D3 · Media | `prototipo/v3/index.html` |
| D4 | Iconos con significado en la barra de pestañas y estado activo. | D4 · Media | `prototipo/v3/index.html` |
| D5 | Foco visible, objetivos de 44 px, foco inicial y Esc en diálogos. | D5 · Baja | `prototipo/v3/index.html` |
| — | Panel del moderador: prepara T1 – T3, mide tiempo, clics y eventos y exporta `resultados.csv`. | Trazabilidad de la prueba | `prototipo/v3/index.html` |
| — | Pago rechazado solo en el primer intento (para T3). | Escenario de prueba | `prototipo/v3/index.html` |

## v3.1 (iteración posterior a la prueba)

| Hallazgo | Cambio aplicado en el prototipo v3.1 | Commit / PR | Responsable |
|---|---|---|---|
| H1 | Se sustituyó «Cancelar» por el texto explícito **«Mantener en el pedido»** en el modal de eliminación y se mantuvo el botón de peligro **«Sí, eliminar»**. | PR #4 (`integral/iteracion`) | Henry Lagua |
| H2 | Se incluyó una línea descriptiva con ingredientes principales (*Pan artesanal, jamón y queso*) en la tarjeta de producto del menú. | PR #4 (`integral/iteracion`) | Melany Cevallos |
| H3 | Se añadió el botón **«Copiar código #A24»** con microinteracción de feedback (*«¡Código copiado!»*) y recordatorio del punto de retiro. | PR #4 (`integral/iteracion`) | Alison Cobos |
