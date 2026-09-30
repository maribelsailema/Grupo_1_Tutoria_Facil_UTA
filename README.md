# Grupo_1_Tutoria_Facil_UTA

> **Tutoría Fácil UTA**: aplicación web móvil para consultar disponibilidad, reservar, confirmar y reprogramar tutorías académicas.
> Prueba práctica integradora · Interacción Humano Computador · Universidad Técnica de Ambato, FISEI, Ingeniería de Software · Quinto semestre.

**Grupo:** N.° 1  **Paralelo:** `A`  **Fecha:** `[30/09/2026]`

---

## 1. Integrantes y roles

| N.° | Integrante | Rol |
| --- | --- | --- |
| 1 | Alex Guachi | Backend |
| 2 | Viviana Sarco | QA (pruebas y evaluación) |
| 3 | Sebastian Santana | Frontend (prototipo y diseño) |
| 4 | Wilson Pillapa | Tester |

---

## 2. Problema de diseño

La Facultad coordina las tutorías mediante WhatsApp, hojas de cálculo y agendas personales. El proceso actual tarda en promedio **14 minutos y 9 mensajes** hasta obtener una confirmación (E4). Además, se registraron **4 confirmaciones ambiguas y 3 intentos de elegir horarios ocupados** en 12 solicitudes (E3), y hay estudiantes que olvidan la fecha porque la confirmación queda mezclada con otros mensajes (E5).

**Pregunta de diseño:** ¿Cómo permitir que un estudiante reserve o reprograme una tutoría desde un teléfono, con claridad, bajo esfuerzo cognitivo, prevención de errores y acceso mediante teclado o tecnologías de apoyo?

**Alcance:** desde que el estudiante busca un horario hasta que obtiene una confirmación comprensible, más la ruta para reprogramar. No incluye autenticación, reportes ni administración de usuarios.

---

## 3. Enlaces

| Recurso | Enlace |
| --- | --- |
| Repositorio | `https://github.com/maribelsailema/Grupo_1_Tutoria_Facil_UTA` |
| Tablero FigJam | `[URL de FigJam con acceso "Cualquier persona con el enlace puede ver"]` |
| PDF del tablero FigJam | [`docs/tablero_figjam_completo.pdf`](docs/tablero_figjam_completo.pdf) |
| Prototipo navegable (Figma/Penpot) | `[URL del prototipo con acceso de solo lectura]` (ver [`prototipo/enlace_prototipo.md`](prototipo/enlace_prototipo.md)) |
| Prueba e iteración | [`test/prueba_iteracion.md`](evaluacion/prueba_iteracion.md) |


---


### Mapa de evidencias

| Actividad | Evidencia | Ubicación |
| --- | --- | --- |
| Fundamentos de IHC | Matriz humano-sistema con E1 a E10 | `docs/01_matriz_ihc.pdf` |
| Usabilidad y accesibilidad | Indicadores, metas y cuatro decisiones POUR | `docs/02_usabilidad_accesibilidad.pdf` |
| DCU | Contexto, persona, escenario, journey map y cinco requisitos | `docs/03_dcu_contexto.pdf` |
| Decisiones de diseño | Metáforas, affordance, mapeo, Gestalt y guía de estilo | `docs/04_decisiones_diseno.pdf` |
| Prototipo | Cuatro pantallas y enlace navegable | `prototipo/` |
| Prueba e iteración | Tarea, medidas, hallazgo, antes y después | `evaluacion/prueba_iteracion.md` |
| Trabajo colaborativo | Issues, ramas, commits, PR y revisiones | Pestañas *Issues*, *Pull requests* y *Commits* |

---

## 5. Resumen de la iteración

**Prueba cruzada:** Wilson Pillapa, estudiante de quinto semestre de Ingeniería de Software (paralelo A), recibió el prototipo sin explicación previa y realizó en computadora la tarea *"Reserva una tutoría para el jueves y luego cambia el horario"*.

| Aspecto | Resultado |
| --- | --- |
| Reserva completada sin ayuda | Sí |
| Cambio de horario completado sin ayuda | Sí |
| Tiempo total aproximado | ≈ 2:10 (proceso actual: 14 min, E4) |
| Errores observados | 0 |
| Satisfacción | 7 de 7 |
| Hallazgo principal | El flujo se comprendió sin ayuda; al reprogramar, la pantalla no mostraba el horario anterior ni permitía deshacer (E5, E10) |

**Mejora aplicada:** en la Pantalla 4 se agregó el mensaje "Tutoría reprogramada", un resumen "Antes / Ahora" y el botón "Deshacer cambio".

| | Antes | Después |
| --- | --- | --- |
| Pantalla afectada | Pantalla 4 | Pantalla 4 |
| Resultado | El cambio se reflejaba sin resumen ni opción de deshacer | Cambio explícito con "Antes / Ahora" y recuperación con un clic (verificación teórica) |

Detalle completo en [`evaluacion/prueba_iteracion.md`](evaluacion/prueba_iteracion.md).

---

## 6. Flujo de colaboración aplicado

1. **Planificar:** repositorio creado, 4 integrantes registrados y un issue asignado a cada uno.
2. **Desarrollar:** una rama `feature/nombre-aporte` por integrante, con al menos dos commits que describen cambios concretos.
3. **Revisar:** un pull request por integrante, revisado por un compañero distinto.
4. **Integrar:** los tres PR aprobados y fusionados en `main`; enlaces y carpetas verificados.

---

## 7. Control final

- [ ] El repositorio abre sin solicitar permisos adicionales (docente con acceso de lectura).
- [ ] `main` contiene README, `docs/`, `prototipo/` y `test/`.
- [ ] Los tres issues están cerrados o vinculados a su PR.
- [ ] Los tres PR están revisados y fusionados.
- [ ] Cada integrante identifica su trabajo en el historial.
- [ ] Enlaces de FigJam, PDF y prototipo verificados en ventana privada.
