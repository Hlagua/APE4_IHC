# PRÁCTICA EXPERIMENTAL DE APRENDIZAJE – APE 4
## Caso CaféU: Prototipado, Wireframes, Evaluación con Usuarios e Iteración Refinada

![Universidad Técnica de Ambato](https://img.shields.io/badge/UTA-FISEI-red?style=flat-square)
![Asignatura](https://img.shields.io/badge/Asignatura-Interacci%C3%B3n_Humano--Computador-blue?style=flat-square)
![Semestre](https://img.shields.io/badge/Nivel-Quinto_A-informational?style=flat-square)
![Periodo](https://img.shields.io/badge/Periodo-Julio_--_Diciembre_2026-green?style=flat-square)

---

### Información Académica
- **Institución:** Universidad Técnica de Ambato (UTA)
- **Facultad:** Facultad de Ingeniería en Sistemas, Electrónica e Industrial (FISEI)
- **Carrera:** Ingeniería de Software
- **Docente:** Ing. José Rubén Caiza Caizabuano, Mg.
- **Caso de Estudio:** **CaféU** — Aplicación web móvil para la gestión y anticipación de pedidos en la cafetería universitaria.

---

### Integrantes Oficiales del Equipo y Roles

| Integrante | Usuario GitHub | Correo Institucional / Contacto | Rol Oficial en el Proyecto |
|---|---|---|---|
| **Alison Marcela Cobos Taco** | [@Itsuna18](https://github.com/Itsuna18) | tacomarcelab@gmail.com | **Desarrollador Back-End** (Modelos de datos, lógica de interacción y estados del prototipo, persistencia y validaciones) |
| **Melany Saleth Cevallos Goyes** | [@SalyC15](https://github.com/SalyC15) | mcevallos8901@uta.edu.ec | **Desarrollador Front-End** (Diseño en Figma, inventario UI, pantallas refinadas y componentes visuales v3/v3.1) |
| **Carlos Giovanni Ramos Jácome** | [@carlitosgiovanniramos](https://github.com/carlitosgiovanniramos) | carlos.giovanni.ramos.work@gmail.com | **Tester** (User flows, protocolos de validación, evaluación con usuarios P01/P02, métricas y matriz de hallazgos) |
| **Henry Daniel Lagua Flores** | [@Hlagua](https://github.com/Hlagua) | hlagua6116@uta.edu.ec | **QA / Arquitecto** (Arquitectura de información, especificación de microinteracciones, iteración v3.1, auditorías e informes finales) |

---

### Entregas del Proyecto

El repositorio consolida las tres etapas de la práctica:

1. **[APE 4 Integral (Entrega Final Consolidada)](APE4-integral/)**
2. **[APE 4 Fase 2 (Prototipado Refinado y Prueba Inicial)](APE4_Fase2/)**
3. **[APE 4 Fase 1 (Requisitos, Arquitectura y Wireframes)](APE4_Fase1/)**

---

### Entrega Integral APE 4 (`APE4-integral/`)

Carpeta contenedora: [`APE4-integral/`](APE4-integral/) · **[Ver README de la versión integral](APE4-integral/README.md)**

| Fase de la guía | Evidencia | Descripción |
|---|---|---|
| **1. Diagnóstico** | [`APE4-integral/diagnostico.md`](APE4-integral/diagnostico.md) | Análisis del usuario universitario, sitemap, user flow y 5 problemas priorizados con severidad Nielsen y WCAG. |
| **2. Construcción** | [`APE4-integral/prototipo/v3/`](APE4-integral/prototipo/v3/) | Prototipo navegable v3 de 8 pantallas con flujos de pedido, modificación, pago y seguimiento. |
| **3. Prueba de Usabilidad** | [`APE4-integral/pruebas/`](APE4-integral/pruebas/) | Protocolo de observación, ejecución con usuarios P01 y P02, registro en `resultados.csv` y 3 hallazgos priorizados (`hallazgos.md`). |
| **4. Iteración y Mejora** | [`APE4-integral/iteracion/`](APE4-integral/iteracion/) · [`prototipo/v3.1/`](APE4-integral/prototipo/v3.1/) | Prototipo refinado v3.1 con badge/limpieza de filtros, confirmación destructiva y desglose dinámico en checkout. |
| **5. Conclusiones y Defensa** | [`APE4-integral/conclusiones.md`](APE4-integral/conclusiones.md) · [`colaboracion.md`](APE4-integral/colaboracion.md) | Conclusiones técnicas, respuestas a la defensa de la guía y trazabilidad colaborativa en GitHub (Issues, ramas y PRs). |
| **Informe Oficial** | [`APE4-integral/informe/APE4_Integral_CafeU.pdf`](APE4-integral/informe/APE4_Integral_CafeU.pdf) | Documento formal de la práctica con formato UTA y bibliografía en norma IEEE. |

---

### Entregables de la Fase 2 (`APE4_Fase2/`)

Carpeta contenedora: [`APE4_Fase2/`](APE4_Fase2/)

| N.º | Entregable Oficial | Ubicación en el Repositorio | Descripción |
|---|---|---|---|
| **1** | **Pantallas refinadas y comparativa** | [`APE4_Fase2/01_pantallas_refinadas/`](APE4_Fase2/01_pantallas_refinadas/) | 19 vistas refinadas (R1 a R7, estados y variantes) y comparativa visual directa en [`comparativa_fase1_fase2/`](APE4_Fase2/01_pantallas_refinadas/comparativa_fase1_fase2/). |
| **2** | **Prototipo interactivo navegable** | [Figma Fase 2](https://www.figma.com/proto/0bxGDlHenLKFwC9IroyRXt?node-id=12-91&starting-point-node-id=12%3A91) · [`02_prototipo/index.html`](APE4_Fase2/02_prototipo/index.html) | Prototipo web interactivo refinado con máquina de estados, marco de dispositivo móvil y panel de pruebas. |
| **3** | **Estados del sistema y microinteracciones** | [`APE4_Fase2/03_estados_microinteracciones/`](APE4_Fase2/03_estados_microinteracciones/) | Los 4 estados de la interfaz (inicial, procesamiento, error, éxito), matriz de validaciones y catálogo de 5 microinteracciones documentadas. |
| **4** | **Guion y matriz de prueba cognitiva** | [`APE4_Fase2/04_prueba_cognitiva/guion_y_matriz_de_prueba.md`](APE4_Fase2/04_prueba_cognitiva/guion_y_matriz_de_prueba.md) | Protocolo ejecutado con dos compañeros externos (tareas T1 y T2, roles del equipo y matriz de resultados). |
| **5** | **Hallazgos y recomendaciones** | [`APE4_Fase2/05_hallazgos_recomendaciones.md`](APE4_Fase2/05_hallazgos_recomendaciones.md) | Priorización de los 3 hallazgos detectados en la prueba cognitiva y justificación ergonómica de las correcciones. |
| **6** | **Versiones antes y después** | [`APE4_Fase2/06_antes_despues/`](APE4_Fase2/06_antes_despues/) | Comparativas visuales antes y después de aplicar las correcciones sobre el prototipo. |
| **7** | **Documento PDF explicativo** | [`APE4_Fase2/07_documento/APE4_Fase2_CafeU.pdf`](APE4_Fase2/07_documento/APE4_Fase2_CafeU.pdf) | Informe completo en PDF con las cinco actividades, tres conclusiones y bibliografía en formato IEEE. |

---

### Entregables de la Fase 1 (`APE4_Fase1/`)

Carpeta contenedora: [`APE4_Fase1/`](APE4_Fase1/)

| N.º | Entregable Oficial | Ubicación en el Repositorio | Descripción |
|---|---|---|---|
| **1** | **Matriz de requisitos y pantallas** | [`APE4_Fase1/01_matriz_requisitos_pantallas.md`](APE4_Fase1/01_matriz_requisitos_pantallas.md) | Requisitos funcionales (RF-01 a RF-08) y mapeo hacia pantallas W1-W7. |
| **2** | **Sitemap del proyecto** | [`APE4_Fase1/02_sitemap.png`](APE4_Fase1/02_sitemap.png) | Arquitectura de información jerárquica de la cafetería universitaria. |
| **3** | **Dos diagramas User Flow** | [`03_userflow_1_realizar_pedido.png`](APE4_Fase1/03_userflow_1_realizar_pedido.png)<br>[`03_userflow_2_modificar_pedido.png`](APE4_Fase1/03_userflow_2_modificar_pedido.png) | Flujos críticos con caminos felices, puntos de decisión y alternativas de error. |
| **4** | **Esquema de navegación y componentes** | [`APE4_Fase1/04_esquema_navegacion.png`](APE4_Fase1/04_esquema_navegacion.png)<br>[`04_navegacion_e_inventario_componentes.md`](APE4_Fase1/04_navegacion_e_inventario_componentes.md) | Catálogo de componentes y justificación ergonómica (Hick, Fitts, Nielsen). |
| **5** | **Wireframes de baja fidelidad** | [`APE4_Fase1/05_wireframes/`](APE4_Fase1/05_wireframes/) | 7 pantallas principales (W1-W7) y 4 estados críticos (E1-E4). |
| **6** | **Documento explicativo didáctico** | [`APE4_Fase1/06_documento/APE4_Fase1_CafeU.pdf`](APE4_Fase1/06_documento/APE4_Fase1_CafeU.pdf) | Justificación didáctica paso a paso de la Fase 1. |
| **7** | **Prototipo de baja fidelidad** | [Figma Fase 1](https://www.figma.com/proto/0bxGDlHenLKFwC9IroyRXt?node-id=2-4&starting-point-node-id=2%3A4) · [`07_prototipo/index.html`](APE4_Fase1/07_prototipo/index.html) | Prototipo inicial de baja fidelidad. |
| **8** | **Protocolo de pruebas de usabilidad** | [`APE4_Fase1/08_protocolo_pruebas_usabilidad.md`](APE4_Fase1/08_protocolo_pruebas_usabilidad.md) | Casos de prueba CP-01 a CP-05, heurísticas de Nielsen y métricas SUS/SEQ. |

---

### Prototipos en Vivo y Enlaces Oficiales

- **Repositorio en GitHub:** [https://github.com/Hlagua/APE4_IHC](https://github.com/Hlagua/APE4_IHC)
- **Portal de Prototipos (GitHub Pages):** [https://hlagua.github.io/APE4_IHC/](https://hlagua.github.io/APE4_IHC/)
- **Prototipo v3.1 (Iteración Refinada):** [https://hlagua.github.io/APE4_IHC/APE4-integral/prototipo/v3.1/](https://hlagua.github.io/APE4_IHC/APE4-integral/prototipo/v3.1/)
- **Prototipo v3 (Evaluación):** [https://hlagua.github.io/APE4_IHC/APE4-integral/prototipo/v3/](https://hlagua.github.io/APE4_IHC/APE4-integral/prototipo/v3/)
- **Prototipo Fase 2 en Vivo:** [https://hlagua.github.io/APE4_IHC/APE4_Fase2/02_prototipo/](https://hlagua.github.io/APE4_IHC/APE4_Fase2/02_prototipo/)
- **Prototipo Fase 1 en Vivo (Wireframes):** [https://hlagua.github.io/APE4_IHC/APE4_Fase1/07_prototipo/](https://hlagua.github.io/APE4_IHC/APE4_Fase1/07_prototipo/)
- **Figma Oficial (v1 y v2):** [https://www.figma.com/design/0bxGDlHenLKFwC9IroyRXt](https://www.figma.com/design/0bxGDlHenLKFwC9IroyRXt)
