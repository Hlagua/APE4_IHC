# Colaboración en GitHub · APE 4 integral

La guía de la práctica APE 4 exige **al menos una issue por integrante, rama propia, commits descriptivos y un Pull Request revisado por un compañero**. Cada integrante realiza su aporte bajo su identidad y rol oficial en el proyecto.

## Equipo de trabajo y roles

| Integrante | Usuario GitHub | Rol Oficial | Rama asignada | Issue oficial |
|---|---|---|---|---|
| **Alison Marcela Cobos Taco** | [@Itsuna18](https://github.com/Itsuna18) | Desarrollador Back-End | `integral/diagnostico` | [#2 Diagnóstico y tareas de prueba](https://github.com/Hlagua/APE4_IHC/issues/2) |
| **Melany Saleth Cevallos Goyes** | [@SalyC15](https://github.com/SalyC15) | Desarrollador Front-End | `integral/prototipo-v3` | [#3 Prototipo v3 y evidencias](https://github.com/Hlagua/APE4_IHC/issues/3) |
| **Carlos Giovanni Ramos Jácome** | [@carlitosgiovanniramos](https://github.com/carlitosgiovanniramos) | Tester | `integral/prueba` | [#4 Prueba con P01 y P02](https://github.com/Hlagua/APE4_IHC/issues/4) |
| **Henry Daniel Lagua Flores** | [@Hlagua](https://github.com/Hlagua) | QA / Arquitecto | `integral/iteracion` | [#1 Iteración v3.1, README e informe final](https://github.com/Hlagua/APE4_IHC/issues/1) |

---

## Trazabilidad de Pull Requests y Revisiones Cruzadas (Defensa Pregunta 3)

| Integrante | Issue | Rama técnica | Pull Request | Revisor asignado | Estado |
|---|---|---|---|---|---|
| **Alison Cobos** | [#2](https://github.com/Hlagua/APE4_IHC/issues/2) | `integral/diagnostico` | [PR #5 (`integral/diagnostico`)](https://github.com/Hlagua/APE4_IHC/pull/5) | Carlos Ramos (@carlitosgiovanniramos) | Merged |
| **Melany Cevallos** | [#3](https://github.com/Hlagua/APE4_IHC/issues/3) | `integral/prototipo-v3` | [PR #6 (`integral/prototipo-v3`)](https://github.com/Hlagua/APE4_IHC/pull/6) | Alison Cobos (@Itsuna18) | Merged |
| **Carlos Ramos** | [#4](https://github.com/Hlagua/APE4_IHC/issues/4) | `integral/prueba` | [PR #7 (`integral/prueba`)](https://github.com/Hlagua/APE4_IHC/pull/7) | Alison Cobos (@Itsuna18) | Merged |
| **Henry Lagua** | [#1](https://github.com/Hlagua/APE4_IHC/issues/1) | `integral/iteracion` | [PR #8 (`integral/iteracion`)](https://github.com/Hlagua/APE4_IHC/pull/8) | Melany Cevallos (@SalyC15) | Merged |

---

## Detalle de aportes por rama y tareas

### 1. Rama `integral/diagnostico` — Alison Cobos (@Itsuna18)
- **Archivos entregados:** `APE4-integral/diagnostico.md`, `sitemap.png`, `user-flow.png`, `wireframes/`.
- **Aporte:** Análisis de necesidades del estudiante universitario, sitemap jerárquico, user flows para los 3 caminos críticos y priorización de los 5 problemas de diseño (D1 a D5) evaluados con severidad Nielsen y WCAG.
- **Commit:** `docs(diagnostico): formalizar diagnostico de diseno, sitemap, user flow y 5 problemas priorizados (closes #2)`

### 2. Rama `integral/prototipo-v3` — Melany Cevallos (@SalyC15)
- **Archivos entregados:** `APE4-integral/prototipo/v3/`, `evidencias/`, `iteracion/antes-despues.md`.
- **Aporte:** Construcción de prototipo interactivo en HTML de 8 pantallas, capturas de evidencias visuales de los flujos principales y documentación de la comparativa de pantalla inicial.
- **Commit:** `feat(prototipo-v3): implementar prototipo navegable v3 de 8 pantallas, evidencias visuales y comparativa inicial (closes #3)`

### 3. Rama `integral/prueba` — Carlos Ramos (@carlitosgiovanniramos)
- **Archivos entregados:** `APE4-integral/pruebas/protocolo.md`, `pruebas/resultados.csv`, `pruebas/hallazgos.md`.
- **Aporte:** Moderación y registro de la prueba de usabilidad con 2 usuarios externos (P01 y P02) en 3 tareas (T1, T2, T3), recolección de métricas temporales (tiempo, éxito del 100%) y consolidación de 3 hallazgos priorizados (H1, H2, H3).
- **Commit:** `test(evaluacion): registrar protocolo de prueba, matriz de observaciones con P01 y P02 y 3 hallazgos priorizados (closes #4)`

### 4. Rama `integral/iteracion` — Henry Lagua (@Hlagua)
- **Archivos entregados:** `APE4-integral/prototipo/v3.1/`, `iteracion/cambios.md`, `conclusiones.md`, `colaboracion.md`, `informe/APE4_Integral_CafeU.pdf`, `README.md`, `index.html`.
- **Aporte:** Desarrollo de la versión iterada v3.1 resolviendo los 3 hallazgos (badge/limpieza de filtros, modal de confirmación destructiva y desglose dinámico en checkout), redacción de conclusiones, actualización de portal navegable y generación del informe oficial en PDF bajo norma IEEE.
- **Commit:** `fix(iteracion): implementar prototipo v3.1 con 3 correcciones, conclusiones, informe final PDF y consolidacion del repositorio (closes #1)`
