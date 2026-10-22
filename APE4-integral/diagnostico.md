# Diagnóstico · APE 4 integral — CaféU

**Fase 1 de la guía integral (35 min).** Punto de partida: entregas de las carpetas [`APE4_Fase1`](../APE4_Fase1) (requisitos, sitemap, user flows, wireframes v1) y [`APE4_Fase2`](../APE4_Fase2) (diseño refinado y prototipo v2).

> **Asignación del equipo.** El repositorio `Hlagua/APE4_IHC` no figura en la tabla «Asignación contextualizada por repositorio» de la guía. Se toma como reto el más cercano a nuestro caso (CaféU): **probar búsqueda, edición y confirmación del pedido**, y se documenta la decisión para confirmarla con el docente.

## 1. Usuario

| Elemento | Descripción |
|---|---|
| Usuario principal | Estudiante universitario que compra en la cafetería del campus entre clases. |
| Contexto | Descanso corto (10–15 min), fila concurrida, uso desde el celular con una mano. |
| Objetivo | Pedir y pagar sin hacer fila, saber cuándo retirar y corregir el pedido si se equivoca. |
| Riesgos para el usuario | Pagar dos veces, perder el pedido, no encontrar un producto, no saber si la acción funcionó. |

## 2. Tres tareas representativas (base de la prueba)

| Tarea | Tipo pedido por la guía | Consigna para el participante | Éxito |
|---|---|---|---|
| T1 | Localizar un elemento y seleccionar una acción | «Busca el sánduche en el menú y agrégalo a tu pedido.» | El sánduche queda en «Mi pedido» (contador = 1). |
| T2 | Completar o modificar una operación con validación | «Ya no quieres el sánduche. Quítalo de tu pedido y deja 2 cafés.» | Resumen con «Cambios guardados», 2 cafés, $3.00. |
| T3 | Finalizar y verificar la confirmación | «Paga tu pedido. Si algo sale mal, resuélvelo y dinos tu número de pedido.» (el primer pago es rechazado) | Reintenta, llega a «¡Pedido confirmado!» y dice «#A24». |

## 3. Revisión de los wireframes y del prototipo v2

| Artefacto | Coherencia con requisitos y flujos | Observación |
|---|---|---|
| Sitemap (Fase 1) | Coherente: 4 pantallas principales y 3 secundarias. | Se mantiene sin cambios. |
| User flow 1 y 2 (Fase 1) | Coherentes con T1 – T3. | T3 recorre la rama «¿Pago aprobado? No». |
| Wireframes v1 (W1 – W7, E1 – E4) | Cubren las tres tareas. | Base de la v2. |
| Prototipo v2 (Fase 2, HTML y Figma) | Navegable, 3 flujos, 4 estados. | Revisión heurística del equipo → 5 problemas (abajo). |

## 4. Cinco problemas priorizados (revisión heurística del equipo sobre la v2)

Prioridad = gravedad (1–3) × frecuencia esperada en las tareas (1–3).

| N.º | Problema detectado en la v2 | Evidencia | Heurística / criterio | Gravedad | Frec. | Prioridad |
|---|---|---|---|---|---|---|
| D1 | El mensaje de pago rechazado no dice si se cobró; el usuario puede temer un doble cobro. | `evidencias/v2/d1_pago_rechazado.png` | H9 Ayudar a reconocer y recuperarse de errores | 3 | 2 | **6 · Alta** |
| D2 | La búsqueda exige tildes: «sanduche» no encuentra «Sánduche» y muestra «No encontramos…». | `evidencias/v2/d2_busqueda_sin_tilde.png` | H5 Prevención de errores · H2 Lenguaje del usuario | 2 | 3 | **6 · Alta** |
| D3 | Para quitar un producto, «−» se bloquea en 1 y obliga a buscar el botón «Eliminar». | `evidencias/v2/d3_editar_menos.png` | H7 Flexibilidad · H4 Consistencia con apps conocidas | 2 | 2 | **4 · Media** |
| D4 | La barra de pestañas usa cuadros vacíos como iconos: solo se distinguen por la etiqueta. | `evidencias/v2/d4_barra_pestanas.png` | H6 Reconocer antes que recordar · WCAG 1.1.1 | 1 | 3 | **3 · Media** |
| D5 | Accesibilidad: sin foco visible propio para teclado, chips y botón «Eliminar» de ~34 px, diálogos sin foco inicial ni cierre con Esc. | Inspección del código v2 | WCAG 2.4.7 Foco visible · 2.5.8 Tamaño del objetivo · 2.1.1 Teclado | 2 | 1 | **2 · Baja** |

Estos cinco problemas se corrigieron en la fase de **construcción** (prototipo v3); ver [`iteracion/antes-despues.md`](iteracion/antes-despues.md). Las correcciones **posteriores a la prueba** con usuarios se registran por separado en [`iteracion/cambios.md`](iteracion/cambios.md).

---

## 5. Validación del diagnóstico y modelos de datos

**Revisado por Alison Cobos (@Itsuna18) — Desarrollador Back-End:**
«Se validó la consistencia entre los cinco problemas priorizados y la persistencia de datos del prototipo. Específicamente, D1 (garantía explícita de no cobro en el estado de error de pago) previene transacciones huérfanas en el backend y elimina la incertidumbre del usuario, mientras que D2 (normalización de caracteres y búsqueda sin tildes) optimiza las consultas del catálogo sin sobrecargar el filtrado. Las tres tareas T1, T2 y T3 cubren completamente el ciclo de vida del pedido en el cliente.»
