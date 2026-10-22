# Protocolo de prueba de usabilidad y accesibilidad · CaféU v3

**Fase 3 de la guía integral (50 min).** Prototipo evaluado: [`prototipo/v3/index.html`](../prototipo/v3/index.html) (abrirlo en una laptop; el panel del moderador queda a la derecha).

## Participantes

- **Dos personas ajenas al diseño** (no integrantes del equipo), identificadas como **P01** y **P02**. Solo se registran las iniciales o un alias.
- Antes de empezar se les pide permiso para anotar lo que digan y tomar capturas.

## Roles

| Rol | Integrante | Responsabilidad |
|---|---|---|
| Moderador | _______ | Lee la consigna, pulsa «Iniciar» y marca el resultado. **No indica dónde tocar.** |
| Observador | _______ | Escribe en «Observación» las dudas textuales, errores y regresos. |
| Accesibilidad | _______ | Ejecuta la verificación de teclado y contraste (sección 5). |
| Evidencias | _______ | Toma capturas en las pantallas donde hay dudas y las guarda en `evidencias/prueba/`. |

## Procedimiento por participante (≈ 12 min)

1. Escribir el código del participante (P01 o P02) en el panel.
2. Para cada tarea: **Preparar Tn** → leer la consigna en voz alta → **▶ Iniciar** → observar en silencio.
3. Al terminar: **✓ Éxito**, **Con ayuda** o **✗ No completó**; pedir la dificultad del 1 (muy fácil) al 5 (muy difícil) y escribir la observación.
4. El panel mide **tiempo (s)**, **clics** y **eventos** (búsqueda sin resultados, regresos, diálogos cerrados, pago rechazado).
5. Al final de los dos participantes: **⬇ Descargar resultados.csv** y reemplazar [`resultados.csv`](resultados.csv).

## Tareas

| Tarea | Consigna (leer textual) | Estado inicial (botón «Preparar») | Criterio de éxito |
|---|---|---|---|
| T1 | «Busca el sánduche en el menú y agrégalo a tu pedido.» | Inicio, pedido vacío | Sánduche en «Mi pedido». |
| T2 | «Ya no quieres el sánduche. Quítalo de tu pedido y deja 2 cafés.» | «Mi pedido» con 1 café y 1 sánduche | «Cambios guardados», 2 cafés, $3.00. |
| T3 | «Paga tu pedido. Si algo sale mal, resuélvelo y dinos tu número de pedido.» | «Mi pedido» con 2 cafés; el **primer pago se rechaza** | Reintenta y dice «#A24». |

## Heurísticas de Nielsen verificadas durante la prueba

| Heurística | Dónde se observa | Se cumple si… |
|---|---|---|
| H1 · Visibilidad del estado del sistema | T1 (aviso y contador), T3 (procesamiento) | El participante sabe sin preguntar que el producto se agregó y que el pago está en curso. |
| H5 · Prevención de errores | T2 (confirmación al quitar), T3 (botón bloqueado al procesar) | No borra por accidente ni pulsa «Pagar» dos veces. |
| H9 · Reconocer, diagnosticar y recuperarse de errores | T3 (pago rechazado) | Entiende que no se le cobró y usa «Reintentar pago» sin ayuda. |

## Condiciones de accesibilidad verificadas

| Condición | Criterio WCAG 2.2 | Cómo se verifica | Resultado esperado |
|---|---|---|---|
| A1 · Contraste del texto | 1.4.3 (mínimo 4,5:1) | Cálculo de contraste de los colores del sistema visual | Texto principal 16,14:1; secundario 5,58:1; botón primario 8,89:1; error 5,58:1; éxito 5,05:1. Texto de botones desactivados 2,73:1 (exento por ser control inactivo). |
| A2 · Operable con teclado y foco visible | 2.1.1 y 2.4.7 | Completar T2 solo con Tab, Enter y Esc | Todos los controles se alcanzan con Tab, el foco se ve (borde de 3 px), el diálogo recibe el foco y se cierra con Esc. |

Complementario: objetivos táctiles de al menos 44 × 44 px (WCAG 2.5.8) en botones, chips, «Eliminar», pestañas y selector de cantidad.

## Registro

- [`resultados.csv`](resultados.csv): una fila por participante y tarea (participante, tarea, éxito, tiempo_s, clics, eventos, dificultad, observación, fecha).
- [`hallazgos.md`](hallazgos.md): hallazgos con evidencia (fila del CSV y captura) y prioridad.

> No se registran datos de prueba inventados ni ilustrativos: solo lo observado con P01 y P02.
