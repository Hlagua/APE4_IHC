# Hallazgos de la prueba · CaféU v3

Resultados observados durante la prueba con los participantes **P01** (`J. P.`, 22 años) y **P02** (`G. E.`, 21 años) el 22/10/2026.

| N.º | Hallazgo observado | Participante · tarea (fila del CSV) | Heurística o criterio | Gravedad (1–3) | Evidencia | Corrección propuesta |
|---|---|---|---|---|---|---|
| H1 | En T2, la opción «Cancelar» del diálogo al quitar un producto genera duda sobre si cancela solo la eliminación o toda la edición. | P01 · T2 (fila 2) | H5 Prevención · H2 Lenguaje | 2 | Diálogo de eliminación al pulsar «−» en cantidad 1 | Cambiar el texto secundario por «Mantener en el pedido» y «Sí, eliminar». |
| H2 | En T1, el participante ingresó al detalle para comprobar los ingredientes del sánduche antes de agregarlo, sumando pasos innecesarios. | P02 · T1 (fila 4) | H6 Reconocer antes que recordar | 1 | Tarjeta de producto en pantalla Menú | Incluir subtítulo de ingredientes clave («Pan artesanal, jamón y queso») en la tarjeta del menú. |
| H3 | En T3, al confirmarse el pedido, el participante quiso copiar o guardar el código #A24 para mostrarlo en el retiro. | P02 · T3 (fila 6) | H1 Visibilidad del estado · H7 Flexibilidad | 1 | Pantalla de confirmación tras pago exitoso | Agregar botón interactivo «Copiar código #A24» con microinteracción de confirmación en pantalla. |

## Verificación de heurísticas y accesibilidad

| Criterio | P01 | P02 | Observación |
|---|---|---|---|
| H1 · Visibilidad del estado | Cumple | Cumple | El toast verde y el badge «Mi pedido (1)» confirman la acción; la barra de progreso informa el avance del pago. |
| H5 · Prevención de errores | Cumple | Cumple | «−» en 1 no borra directamente, sino que pide confirmación; el botón de pago se bloquea durante el procesamiento. |
| H9 · Recuperación de errores | Cumple | Cumple | El mensaje de pago rechazado explica que no hubo cobro, conserva el pedido y permite reintentar con éxito. |
| A1 · Contraste ≥ 4,5:1 | Cumple (cálculo) | Cumple (cálculo) | Texto 16,14:1; secundario 5,58:1; botón 8,89:1; error 5,58:1; éxito 5,05:1 (WCAG 1.4.3). |
| A2 · Teclado y foco visible | Cumple | Cumple | P02 completó T2 solo con Tab, Enter y Esc; foco visible de 3 px y foco automático en modales (WCAG 2.1.1 y 2.4.7). |
