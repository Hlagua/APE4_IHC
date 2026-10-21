# 04 · Prueba cognitiva rápida con pares — CaféU

**Duración total:** 30 minutos · **Participantes:** 2 compañeros externos al equipo (Quinto semestre, FISEI – UTA) · **Prototipo evaluado:** Figma (*Recorrido 1*, *Recorrido 2* y *Caso de error*) y versión HTML móvil.

## Roles del equipo durante la prueba

| Rol | Integrante asignado | Qué hace |
|---|---|---|
| Moderador | Carlos Giovanni Ramos Jácome | Lee las tareas en voz alta y **no indica dónde hacer clic**. |
| Observador 1 | Alison Marcela Cobos Taco | Anota el recorrido, los clics equivocados y el tiempo empleado. |
| Observador 2 | Melany Saleth Cevallos Goyes | Anota dudas, comentarios en voz alta (*think-aloud*) y la dificultad reportada. |
| Registro | Henry Daniel Lagua Flores | Toma capturas de las pantallas donde ocurren dudas y documenta la evidencia. |

## Guion del moderador

1. «Gracias por ayudarnos. Vamos a probar el diseño de la aplicación, no a ti: si algo no se entiende, es un problema del diseño.»
2. «Mientras usas la aplicación, dinos en voz alta lo que piensas y lo que esperas que pase.»
3. «No te podemos decir dónde tocar; si te quedas atascado, avísanos.»
4. Leer la tarea, abrir el prototipo en el punto de inicio indicado y observar sin intervenir.
5. Al terminar cada tarea, preguntar: «Del 1 (muy fácil) al 5 (muy difícil), ¿qué tan difícil fue?».
6. Al final: «¿Qué fue lo más confuso?» y «¿Qué cambiarías?».

## Tareas evaluadas

| N.º | Tarea leída al participante | Inicio en el prototipo | Criterio de éxito |
|---|---|---|---|
| T1 | «Tienes un descanso corto. Pide un café americano y un sánduche y paga tu pedido.» | Figma: *Recorrido 1* (R1 · Inicio) · HTML: Inicio | Llega a «¡Pedido confirmado!» con #A24 y total $4.25. |
| T2 | «Tu pedido está listo para pagar, pero ya no quieres el sánduche. Quítalo y deja el pedido listo.» | Figma: *Recorrido 2* (R4 · Resumen) · HTML: «Mi pedido» | Vuelve al resumen con «Cambios guardados» y total $1.50. |
| Error (demostración) | Activar «Simular pago rechazado» (HTML) o usar *Caso de error* (Figma) y pedir que pague. | Figma: *Caso de error* | Entiende el mensaje y usa «Reintentar pago». |

## Matriz de registro de prueba ejecutada

**Datos de los participantes:** Usuario 1: `J. P.` (22 años, 5.º semestre Software) · Usuario 2: `G. E.` (21 años, 5.º semestre Software) · **Fecha:** 20/10/2026

| Participante | Tarea | ¿Completó? | Tiempo | Dificultad (1–5) | Errores / dudas observadas | Mejora propuesta |
|---|---|---|---|---|---|---|
| Usuario 1 (`J. P.`) | Tarea 1 | Sí | 48 s | 1 (Muy fácil) | Al agregar el café preguntó: *«¿Ya se guardó en mi pedido?»* antes de ver la barra inferior. | Mostrar aviso verde superior (*toast*) y barra fija con el subtotal acumulado tras agregar cada producto. |
| Usuario 1 (`J. P.`) | Tarea 2 | Sí | 39 s | 2 (Fácil) | Intentó primero bajar la cantidad de 1 a 0 con el botón «−» antes de notar la opción de quitar el ítem. | Acompañar la acción de borrado con un botón de texto explícito «Eliminar» en rojo y hoja de confirmación con el monto a descontar. |
| Usuario 2 (`G. E.`) | Tarea 1 | Sí | 52 s | 1 (Muy fácil) | En el resumen verificó dos veces cuánto se iba a cobrar antes de pulsar confirmar. | Integrar el monto exacto dentro del botón primario («Confirmar y pagar · $4.25»). |
| Usuario 2 (`G. E.`) | Tarea 2 + Error | Sí | 44 s | 2 (Fácil) | Al aparecer el pago rechazado preguntó: *«¿Se me borró el pedido o me cobraron doble?»*. | Explicar en el estado de error que no se realizó ningún cobro y que el pedido sigue intacto antes de «Reintentar pago». |
