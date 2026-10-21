# APE 4 · Fase 2 — Prototipado interactivo, evaluación y mejora UX

**Asignatura:** Interacción Humano-Computador · **Docente:** Ing. José Rubén Caiza Caizabuano · **Nivel:** Quinto – A · UTA FISEI · Julio – diciembre 2026

**Caso:** CaféU (continuación de la Fase 1, carpeta [`../APE4_Fase1`](../APE4_Fase1)).

**Integrantes y Roles Oficiales:**
- **Alison Marcela Cobos Taco** ([@Itsuna18](https://github.com/Itsuna18)) — *Desarrollador Back-End* (Lógica del prototipo interactivo, estados, persistencia y validaciones)
- **Melany Saleth Cevallos Goyes** ([@SalyC15](https://github.com/SalyC15)) — *Desarrollador Front-End* (Diseño refinado en Figma, pantallas refinadas, comparativa visual Fase 1 vs Fase 2)
- **Carlos Giovanni Ramos Jácome** ([@carlitosgiovanniramos](https://github.com/carlitosgiovanniramos)) — *Tester* (Guion de prueba cognitiva rápida con pares, matriz de evaluación y registro de hallazgos)
- **Henry Daniel Lagua Flores** ([@Hlagua](https://github.com/Hlagua)) — *QA / Arquitecto* (Estados de interfaz, microinteracciones, auditoría UX y compilación del informe didáctico)

**Proceso:** Wireframe → diseño refinado → prototipo navegable → estados y feedback → prueba con usuarios → hallazgos → corrección.

## Entregables

| N.º | Entregable | Ubicación | Estado |
|---|---|---|---|
| 1 | Cuatro pantallas refinadas | [`01_pantallas_refinadas/`](01_pantallas_refinadas/) · comparativa en [`comparativa_fase1_fase2/`](01_pantallas_refinadas/comparativa_fase1_fase2/) | Listo |
| 2 | Enlace al prototipo Figma y HTML | Figma: https://www.figma.com/proto/0bxGDlHenLKFwC9IroyRXt?node-id=12-91&starting-point-node-id=12%3A91 · En vivo: https://hlagua.github.io/APE4_IHC/APE4_Fase2/02_prototipo/ · HTML: [`02_prototipo/index.html`](02_prototipo/index.html) | Listo |
| 3 | Estados y microinteracciones | [`03_estados_microinteracciones/`](03_estados_microinteracciones/) | Listo |
| 4 | Matriz de prueba con dos participantes | [`04_prueba_cognitiva/guion_y_matriz_de_prueba.md`](04_prueba_cognitiva/guion_y_matriz_de_prueba.md) | Listo |
| 5 | Hallazgos y recomendaciones | [`05_hallazgos_recomendaciones.md`](05_hallazgos_recomendaciones.md) | Listo |
| 6 | Versiones antes y después | [`06_antes_despues/`](06_antes_despues/) | Listo |
| 7 | PDF explicativo con tres conclusiones | [`07_documento/APE4_Fase2_CafeU.pdf`](07_documento/APE4_Fase2_CafeU.pdf) | Listo |

## Prototipo en Figma

En modo *Presentar* de la página **Fase 2 · Diseño refinado** hay tres flujos:

1. **Recorrido 1 · Pedir un café y un sánduche y pagar** (R1 → R2 → R3 → R2b → R3b → R2c → R4 → R4p → R4q → R6 → R7).
2. **Recorrido 2 · Eliminar el sánduche antes de pagar** (R4 → R5 → R5d → R5b → R4b).
3. **Caso de error · Pago rechazado y reintento** (R4x → R4px → E1 → R4p → R6).

## Prototipo HTML

Abrir [`02_prototipo/index.html`](02_prototipo/index.html) en el navegador o en https://hlagua.github.io/APE4_IHC/APE4_Fase2/02_prototipo/ (también funciona en el celular). El panel lateral permite simular un pago rechazado y reiniciar para cada participante.
