# 05 · Hallazgos y recomendaciones de mejora UX — CaféU

A partir de la prueba cognitiva rápida realizada con dos compañeros externos al equipo (`J. P.` y `G. E.`), se identificaron, priorizaron y corrigieron tres hallazgos clave en el prototipo refinado:

## Matriz de hallazgos priorizados y correcciones aplicadas

| N.º | Hallazgo observado en la prueba | Pantalla afectada | Prioridad | Corrección aplicada | Justificación HCI / Usabilidad |
|---|---|---|---|---|---|
| **H1** | En la Tarea 2, el participante intentó reducir la cantidad de `1` a `0` con el botón «−» porque un icono aislado de basurero resultaba poco evidente para eliminar un ítem completo. | `R5 · Modificar` y `R5d · Confirmar eliminación` | **Alta** | Se desactivó «−» en el límite mínimo (`1`), se colocó un botón explícito con texto y borde rojo **«Eliminar»** junto al selector y se añadió una hoja inferior de confirmación que indica el descuento exacto (`Se quitará $2.75 del total`). | **Reconocer antes que recordar (Nielsen H6), Prevención de errores (H5) y Ley de Fitts:** el texto elimina la ambigüedad del icono y la confirmación evita borrados accidentales. |
| **H2** | En la Tarea 1, tras agregar el primer producto (*Café Americano*), el participante dudó un instante sobre si el producto ya había quedado registrado en su carrito y cuál era el subtotal acumulado. | `R2b · Menú con producto agregado` y `R4 · Resumen` | **Media** | Se incorporó un aviso emergente verde superior (**«✓ Café Americano agregado»**), el contador numérico en la pestaña **«Mi pedido (1)»**, la barra inferior **«Ver mi pedido · $1.50»** y el monto dentro del botón de cobro (**«Confirmar y pagar · $4.25»**). | **Visibilidad del estado del sistema (Nielsen H1) y Reducción de carga cognitiva:** el estudiante recibe confirmación visual inmediata sin tener que recordar ni sumar mentalmente los precios. |
| **H3** | Durante la simulación del fallo de pago, la participante expresó temor de que su pedido se hubiera perdido o de sufrir un doble cobro al volver a intentar. | `E1 · Pago rechazado` y `R4p/R4q · Procesando` | **Media** | Durante el procesamiento se bloquean el botón y el regreso (`‹`) con la leyenda *«No cierres la aplicación»*, y en `E1` se detalla qué ocurrió, que **no se realizó ningún cobro**, que el pedido sigue guardado y se ofrece el botón directo **«Reintentar pago»**. | **Ayuda a reconocer, diagnosticar y recuperarse de errores (Nielsen H9):** el mensaje explica la causa en lenguaje claro, garantiza la integridad del pedido y ofrece una salida inmediata. |

## Evidencia visual Antes / Después

Las comparativas visuales de las tres correcciones aplicadas se encuentran en la carpeta [`06_antes_despues/`](06_antes_despues/):

1. [`06_antes_despues/01_hallazgo_eliminar.png`](06_antes_despues/01_hallazgo_eliminar.png) — Acción «Eliminar» explícita y confirmación con monto descontado.
2. [`06_antes_despues/02_hallazgo_feedback_agregar.png`](06_antes_despues/02_hallazgo_feedback_agregar.png) — Confirmación inmediata al agregar producto y monto visible en el control de acción.
3. [`06_antes_despues/03_hallazgo_pago_rechazado.png`](06_antes_despues/03_hallazgo_pago_rechazado.png) — Mensaje constructivo en pago rechazado con conservación del pedido.
