# 🎓 Tutoría Fácil UTA

> **Prueba práctica integradora del primer parcial**  
> **Asignatura:** Interacción Humano Computador (IHC)  
> **Institución:** Universidad Técnica de Ambato | FISEI | Carrera de Software  
> **Semestre:** Quinto semestre, paralelo "A"  
> **Repositorio:** `Grupo_1_Tutoria_Facil_UTA`  
> **Grupo:** 1

---

## 👥 1. Integrantes, usuarios de GitHub y roles

| N.º | Integrante | Usuario GitHub | Correo institucional | Jerarquía en el equipo | Rol en la prueba |
| :---: | --- | --- | --- | --- | --- |
| **1** | **Sarco Sailema Viviana Maribel** | [@maribelsailema](https://github.com/maribelsailema) | `vsarco7769@uta.edu.ec` | QA | **Analista DCU** |
| **2** | **Pillapa Tubón Wilson Joseph** | [@W1LSONN](https://github.com/W1LSONN) | `wpillapa8482@uta.edu.ec` | Tester | **Diseño y accesibilidad** |
| **3** | **Santana Durán Sebastián Israel** | [@Sebaslsd](https://github.com/Sebaslsd) | `ssantana1312@uta.edu.ec` | Desarrollador Frontend | **Prototipado** |
| **4** | **Guachi Aucapiña Alex Fabricio** | [@A1EXF6A](https://github.com/A1EXF6A) | `aguachi4414@uta.edu.ec` | Desarrollador Backend | **Evaluación e integración** |

### 📌 Responsabilidad principal de los roles en la prueba

- **Analista DCU:** organiza evidencias, contexto de uso, persona, escenario, *journey map* y requisitos.
- **Diseño y accesibilidad:** define indicadores de usabilidad, principios POUR, metáforas, principios Gestalt y guía de estilo.
- **Prototipado:** construye conexiones, flujos navegables y componentes de interfaz en Figma.
- **Evaluación e integración:** ejecuta la prueba de iteración, documenta los hallazgos y consolida la documentación final.

> **Nota:** La asignación de un rol no limita la colaboración. Los integrantes tienen actividad propia registrada en el historial de contribuciones del repositorio.

---

## 🎯 2. Problema de diseño

Actualmente, la Facultad coordina las tutorías académicas mediante mensajes de WhatsApp, hojas de cálculo y agendas personales. El estudiante escribe al docente, espera una respuesta, propone horarios y solicita una confirmación.

Si necesita cambiar la cita, debe iniciar un nuevo intercambio de mensajes. No existe un sistema interactivo unificado que permita gestionar este proceso de forma clara y eficiente.

### 🎯 Reto

Diseñar desde cero **Tutoría Fácil UTA**, una aplicación web con enfoque móvil que permita:

- Consultar la disponibilidad de tutorías.
- Seleccionar una fecha y un horario.
- Reservar una tutoría académica.
- Recibir una confirmación comprensible.
- Reprogramar una tutoría existente.

### ❓ Pregunta de diseño

> **¿Cómo permitir que un estudiante reserve o reprograme una tutoría desde un teléfono, con claridad, bajo esfuerzo cognitivo, prevención de errores y acceso mediante teclado o tecnologías de apoyo?**

### 📌 Alcance

La tarea comienza cuando el estudiante desea buscar un horario y termina cuando obtiene una confirmación comprensible de la reserva o reprogramación.

**No se diseñan:** autenticación, reportes ni administración de usuarios.

---

## 🔗 3. Enlaces del proyecto

- 🎨 **Tablero FigJam:** [Ver tablero en FigJam](docs/) *(actualizar con el enlace público definitivo)*
- 📱 **Prototipo interactivo (Figma / Penpot):** [Ver prototipo](https://app.visily.ai/projects/a97294e6-8e73-4edd-b6f6-c3235bb2de9c/boards/2730988/presenter?play-mode=All+screens)
- 💻 **Repositorio GitHub:** [Grupo_1_Tutoria_Facil_UTA](https://github.com/maribelsailema/Grupo_1_Tutoria_Facil_UTA)

> **Verificación:** Antes de la entrega final, todos los enlaces deben comprobarse en una ventana privada para verificar que puedan abrirse sin solicitar permisos adicionales.

---

## 📁 4. Estructura del repositorio

```text
Grupo_1_Tutoria_Facil_UTA/
├── README.md
├── docs/
│   ├── 01_matriz_ihc.pdf
│   ├── 02_usabilidad_accesibilidad.pdf
│   ├── 03_dcu_contexto.pdf
│   └── 04_decisiones_diseno.pdf
├── prototipo/
│   ├── capturas/
│   └── enlace_prototipo.md
└── evaluacion/
    └── prueba_iteracion.md
```

### 🗺️ Mapa de evidencias

| Actividad | Evidencia | Ubicación |
| --- | --- | --- |
| **Fundamentos de IHC** | Matriz humano-sistema con evidencias E1 a E10 | `docs/01_matriz_ihc.pdf` |
| **Usabilidad y accesibilidad** | Indicadores, metas y cuatro decisiones POUR | `docs/02_usabilidad_accesibilidad.pdf` |
| **DCU** | Contexto, persona, escenario, *journey map* y 5 requisitos | `docs/03_dcu_contexto.pdf` |
| **Decisiones de diseño** | Metáforas, *affordance*, mapeo, Gestalt y guía de estilo | `docs/04_decisiones_diseno.pdf` |
| **Prototipo** | Capturas de cuatro pantallas y enlace navegable | `prototipo/capturas/` y `prototipo/enlace_prototipo.md` |
| **Prueba e iteración** | Tarea, medida, hallazgo y comparación antes/después | `evaluacion/prueba_iteracion.md` |
| **Trabajo colaborativo** | Issue, rama, commits, PR propio y revisión cruzada de otro PR | Historial, Issues y Pull Requests |

---

## 🔄 5. Resumen de la iteración

**Prueba cruzada:** Wilson Pillapa, estudiante de quinto semestre de Ingeniería de Software (paralelo A), recibió el prototipo sin explicación previa y realizó en computadora la tarea:

> *"Reserva una tutoría para el jueves y luego cambia el horario".*

### 📊 Resultados de la prueba

| Aspecto | Resultado |
| --- | --- |
| Reserva completada sin ayuda | Sí |
| Cambio de horario completado sin ayuda | Sí |
| Tiempo total aproximado | ≈ 2:10 (proceso actual: 14 min, E4) |
| Errores observados | 0 |
| Satisfacción | 7 de 7 |
| Hallazgo principal | El flujo se comprendió sin ayuda; al reprogramar, la pantalla no mostraba el horario anterior ni permitía deshacer |

### 💡 Mejora aplicada

En la **Pantalla 4** se agregó el mensaje **"Tutoría reprogramada"**, un resumen **"Antes / Ahora"** y el botón **"Deshacer cambio"**.

De esta manera, el estudiante puede identificar claramente que la reprogramación fue realizada, comparar el horario anterior con el nuevo y disponer de una opción para revertir el cambio.

### 🔍 Comparación antes y después

| | Antes | Después |
| --- | --- | --- |
| **Pantalla afectada** | Pantalla 4 | Pantalla 4 |
| **Resultado** | El cambio se reflejaba sin resumen ni opción de deshacer | Cambio explícito con "Antes / Ahora" y recuperación con un clic (verificación teórica) |

> El detalle completo de la prueba, el hallazgo y las evidencias de la iteración se encuentra en `evaluacion/prueba_iteracion.md`.

---

## 🌿 6. Flujo de colaboración en GitHub

El equipo utilizó un flujo de trabajo basado en **Issues, ramas, commits, Pull Requests y revisión cruzada entre pares**.

### 📌 Proceso de colaboración

1. **Planificar:** se creó el repositorio y se asignó un *issue* a cada integrante.
2. **Desarrollar:** cada integrante trabajó en una rama `feature/nombre-aporte` y realizó al menos dos commits sustanciales relacionados con su *issue*.
3. **Crear Pull Request:** cada integrante creó un PR propio para integrar su trabajo.
4. **Revisar:** cada PR fue revisado por un compañero diferente al autor.
5. **Integrar:** después de la revisión y aprobación, los PR fueron fusionados con la rama `main`.
6. **Verificar:** se realizó la revisión final del `README.md`, las carpetas, las evidencias y los enlaces.

### 🔄 Revisión cruzada de Pull Requests

La revisión se organizó de forma cruzada entre los integrantes:

- **Sebastián revisó el PR #6 de Viviana.**
- **Viviana revisó el PR #5 de Sebastián.**
- **Wilson revisó el PR #8 de Alex.**
- **Alex revisó el PR #7 de Wilson.**

De esta manera, cada integrante realizó su propio aporte y participó en la revisión del trabajo de otro compañero antes de su integración en `main`.

### 📊 Registro del equipo en GitHub

| Integrante y usuario | Issue asignado | Rama | PR propio | PR revisado | Revisión realizada a | Aporte verificable |
| --- | :---: | --- | :---: | :---: | --- | --- |
| **Sarco Viviana**<br>`@maribelsailema` | **#1** | `feature/analisis-dcu` | **PR #6** | **PR #5** | Sebastián | Matriz IHC, contexto de uso, persona, *journey map* y 5 requisitos (`docs/01_matriz_ihc.pdf`, `docs/03_dcu_contexto.pdf`) |
| **Pillapa Wilson**<br>`@W1LSONN` | **#2** | `feature/diseno-accesibilidad` | **PR #7** | **PR #8** | Alex | Indicadores de usabilidad ISO 9241-11, principios POUR y decisiones de diseño (`docs/02_usabilidad_accesibilidad.pdf`, `docs/04_decisiones_diseno.pdf`) |
| **Santana Sebastián**<br>`@Sebaslsd` | **#3** | `feature/prototipo-figma` | **PR #5** | **PR #6** | Viviana | Prototipo interactivo navegable de 4 pantallas y captura de evidencias (`prototipo/capturas/`, `prototipo/enlace_prototipo.md`) |
| **Guachi Alex**<br>`@A1EXF6A` | **#4** | `feature/evaluacion-readme` | **PR #8** | **PR #7** | Wilson | Prueba cruzada de iteración, integración del `README.md` final y exportación de evidencias FigJam (`evaluacion/prueba_iteracion.md`) |

---

## 🛠️ 7. Herramientas utilizadas

| Herramienta | Uso en el proyecto |
| --- | --- |
| **FigJam** | Análisis, mapas conceptuales, organización de evidencias y diagramación |
| **Figma Design / Penpot** | Guía de estilo, diseño UI/UX y prototipado interactivo |
| **GitHub** | Gestión de Issues, ramas, Pull Requests, revisiones e integración |
| **GitHub Desktop** | Control de versiones, commits, sincronización y gestión de ramas |

---

## ♿ 8. Criterios de diseño considerados

El diseño de **Tutoría Fácil UTA** considera diferentes principios y conceptos estudiados en Interacción Humano-Computador:

- **Usabilidad:** eficacia, eficiencia y satisfacción.
- **Accesibilidad:** aplicación de los principios POUR: perceptible, operable, comprensible y robusto.
- **Diseño Centrado en el Usuario (DCU):** contexto de uso, persona, escenario y *journey map*.
- **Prevención de errores:** confirmaciones y comunicación clara del estado del sistema.
- **Recuperación ante errores:** posibilidad de deshacer una reprogramación.
- **Consistencia visual:** aplicación de una guía de estilo común.
- **Principios Gestalt:** organización y agrupación visual de elementos relacionados.
- **Affordance:** elementos de interfaz que permiten comprender las acciones disponibles.
- **Mapeo:** correspondencia clara entre las acciones del usuario y los resultados del sistema.

---

## ✅ 9. Lista de verificación final

- [x] Cada conclusión importante cita al menos una evidencia **E1 a E10**.
- [x] Los indicadores tienen **métrica y meta**.
- [x] Las cuatro decisiones **POUR** pueden comprobarse en el prototipo.
- [x] La **persona** y el **journey map** describen el problema actual.
- [x] Los **cinco requisitos** se relacionan con evidencia y pantalla.
- [x] Las **cuatro pantallas** completan la reserva y permiten iniciar la reprogramación.
- [x] Existe un **hallazgo observado** durante la prueba.
- [x] Existe una **mejora aplicada** a partir del hallazgo.
- [x] Se documentó la comparación **Antes / Después**.
- [x] Cada integrante tiene **issue, rama, dos commits sustanciales y un Pull Request propio**.
- [x] Cada integrante realizó la **revisión cruzada de un Pull Request de otro compañero**.
- [x] **Sebastián revisó el PR #6 de Viviana y Viviana revisó el PR #5 de Sebastián.**
- [x] **Wilson revisó el PR #8 de Alex y Alex revisó el PR #7 de Wilson.**
- [x] Ningún integrante revisó su propio Pull Request.
- [x] Los Pull Requests fueron revisados antes de fusionarse con `main`.


---

## 📚 10. Evidencias del proyecto

La documentación del proyecto se encuentra distribuida entre las carpetas `docs/`, `prototipo/` y `evaluacion/`.

Para revisar el proceso completo se recomienda consultar las evidencias en el siguiente orden:

1. `docs/01_matriz_ihc.pdf`
2. `docs/02_usabilidad_accesibilidad.pdf`
3. `docs/03_dcu_contexto.pdf`
4. `docs/04_decisiones_diseno.pdf`
5. `prototipo/enlace_prototipo.md`
6. `evaluacion/prueba_iteracion.md`

---

## 🏫 Información académica

**Universidad Técnica de Ambato**  
**Facultad de Ingeniería en Sistemas, Electrónica e Industrial (FISEI)**  
**Carrera de Software**  
**Interacción Humano Computador**  
**Quinto semestre — Paralelo "A"**

---

> **Tutoría Fácil UTA** — Prototipo académico desarrollado para aplicar fundamentos de IHC, usabilidad, accesibilidad, Diseño Centrado en el Usuario, prototipado y evaluación iterativa.
