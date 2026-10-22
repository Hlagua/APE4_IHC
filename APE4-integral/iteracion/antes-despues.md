# Antes y después · CaféU

## A. Construcción: correcciones del diagnóstico (v2 → v3)

Corrigen los cinco problemas de [`diagnostico.md`](../diagnostico.md). Código: [`prototipo/v2`](../prototipo/v2/index.html) → [`prototipo/v3`](../prototipo/v3/index.html).

| N.º | Antes (v2) | Después (v3) | Justificación | Evidencia |
|---|---|---|---|---|
| D1 | «No se pudo procesar el pago. Tu pedido se conserva…» | «**El pago no se completó.** No se realizó ningún cobro y tu pedido sigue guardado…» | H9: explicar qué pasó y qué no pasó elimina el temor al doble cobro. | ![D1](d1_pago_rechazado.png) |
| D2 | «sanduche» → «No encontramos «sanduche»» | La búsqueda ignora tildes y mayúsculas y busca también en la descripción («jamón» encuentra el sánduche). | H5 y H2: el sistema se adapta a cómo escribe el usuario en el celular. | ![D2](d2_busqueda_sin_tilde.png) |
| D3 | «−» desactivado en 1 | «−» en 1 abre «¿Eliminar Sánduche del pedido?» con el monto. | H7 y H4: patrón habitual de las apps de compras, con la confirmación como prevención de errores (H5). | ![D3](d3_editar_menos.png) ![D3b](d3_confirmacion.png) |
| D4 | Cuadros vacíos en la barra de pestañas | 🏠 Inicio, ☕ Menú, 🛍️ Mi pedido, 🧾 Mis pedidos, con indicador de pestaña activa y `aria-current`. | H6 y WCAG 1.1.1: el icono refuerza la etiqueta; el lector de pantalla anuncia «Mi pedido, 2 productos». | ![D4](d4_barra_pestanas.png) |
| D5 | Foco por defecto del navegador; chips de ~34 px; diálogo sin foco ni Esc | Foco visible de 3 px; chips, «Eliminar» y enlaces de 44 px; el diálogo recibe el foco y se cierra con Esc. | WCAG 2.4.7, 2.5.8 y 2.1.1. | Código v3 (CSS `:focus-visible`, `min-height: 44px`). |

## B. Iteración: correcciones basadas en la prueba (v3 → v3.1)

A partir de la prueba con P01 y P02 ([`pruebas/hallazgos.md`](../pruebas/hallazgos.md)), se aplicaron tres mejoras en el prototipo v3.1 ([`cambios.md`](cambios.md)):

| N.º | Antes (v3) | Después (v3.1) | Justificación HCI |
|---|---|---|---|
| **H1** | Botón secundario «Cancelar» en el diálogo modal de confirmación al presionar «−» en cantidad 1. | Botón explícito **«Mantener en el pedido»** junto a «Sí, eliminar». | **H5 Prevención de errores y H2 Lenguaje del usuario:** elimina la ambigüedad sobre si se cancela la eliminación o toda la edición. |
| **H2** | Tarjeta de menú muestra únicamente título («Sánduche de jamón y queso») sin detalle de ingredientes. | Se añade subtítulo informativo: *«Pan artesanal, jamón seleccionado y queso mozzarella»*. | **H6 Reconocer antes que recordar:** evita pasos redundantes de exploración hacia la pantalla de detalle. |
| **H3** | Pantalla de confirmación muestra el código `#A24` como texto plano. | Se agrega el botón interactivo **«Copiar código #A24»** con microinteracción de confirmación. | **H1 Visibilidad del estado y H7 Flexibilidad:** facilita al estudiante presentar el código al retirar en el Edificio Central. |
