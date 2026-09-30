# Prueba cruzada e iteración · Tutoría Fácil UTA

**Grupo:** 1  ·  

---

## 1. Diseño de la prueba

| Elemento | Detalle |
| --- | --- |
| Objetivo | Evaluar si una persona ajena al equipo puede reservar una tutoría y reprogramarla sin recibir explicaciones. |
| Método | Prueba de usabilidad con un participante, sin ayuda previa, pensando en voz alta. |
| Dispositivo | Computadora (navegador de escritorio) |
| Consigna entregada (textual) | *"Reserva una tutoría para el jueves y luego cambia el horario."* |
| Reglas del observador | No explicar la interfaz, no guiar y no corregir. Solo observar, cronometrar y anotar. |
| Alcance | Pantallas 1 a 4 del prototipo. |

## 2. Participante

| Dato | Valor |
| --- | --- |
| Código | P1 |
| Nombre | Wilson Pillapa |
| Equipo / curso | Otro equipo · Quinto semestre de Ingeniería de Software, paralelo A |
| Conocimiento previo del prototipo | Ninguno |
| Observadores | Viviana Sarco (QA, responsable del registro); Ariel Cholota (apoyo) |

---

## 3. Matriz de resultados de la prueba (versión 1)

| Tarea | Participante | Resultado | Tiempo | Errores / dudas observables | Hallazgo | Evidencia |
| --- | --- | --- | --- | --- | --- | --- |
| T1. Reservar una tutoría para el jueves | P1 | Completó sin ayuda | ≈ 1:10 | Ninguno | Comprendió el flujo de búsqueda, selección de horario y confirmación sin explicaciones. | E3, E9 |
| T2. Cambiar el horario de la cita | P1 | Completó sin ayuda | ≈ 1:00 | Ninguno | Localizó el cambio de horario, pero la pantalla no muestra un resumen de qué horario se reemplazó. | E5, E10 |
| **Total** | P1 | 2 de 2 sin ayuda | ≈ 2:10 | 0 errores | | Proceso actual: 14 min (E4) |


**Comentario final del participante:**
> "El flujo es claro e intuitivo. Pude reservar la tutoría y cambiar el horario sin ayuda, y en todo momento entendí en qué paso estaba y qué debía hacer. Me pareció fácil de usar."

**Satisfacción (escala 1 a 7):** 7

### Contraste con las metas de usabilidad (Actividad 2)

| Dimensión | Indicador y forma de medir | Meta | Resultado v1 | ¿Cumple? |
| --- | --- | --- | --- | --- |
| Efectividad | Porcentaje de tareas completadas sin ayuda | 100 % | 100 % (2 de 2) | Sí |
| Eficiencia | Tiempo total para reservar y reprogramar | ≤ 3 min | ≈ 2:10 (85 % menos que los 14 min actuales, E4) | Sí |
| Satisfacción | Valoración posterior a la tarea (1 a 7) | ≥ 5 | 7 | Sí |
| Aprendizaje y errores | Errores en el primer intento y recuperación | ≤ 1 error | 0 errores; completó al primer intento | Sí |


---

## 4. Hallazgos

La prueba mostró que el flujo principal es comprensible. Los hallazgos siguientes combinan lo observado con las condiciones de la prueba.

| N.° | Hallazgo | Tipo | Evidencia del caso | Principio relacionado | Severidad |
| --- | --- | --- | --- | --- | --- |
| H1 | El participante completó reserva y reprogramación sin ayuda, sin errores y con satisfacción 7. | Fortaleza | E3, E4, E9 | Efectividad, consistencia, reconocimiento antes que recuerdo | No aplica |
| H2 | Al cambiar el horario, la pantalla actualiza la cita pero no muestra explícitamente el horario anterior ni permite deshacer el cambio. | Oportunidad de mejora | E5, E10 | Retroalimentación, recuperación de errores, carga cognitiva (no obliga a memorizar) | Media |
| H3 | La prueba se hizo en computadora, aunque el contexto real es móvil con conexión variable. | Limitación | E1, E8 | Validez del contexto de uso | Media |
| H4 | No se comprobó el uso solo con teclado ni con lector de pantalla. | Limitación | E2 | Accesibilidad operable y robusta (POUR) | Media |

**Hallazgo priorizado para la iteración: H2.** Es el único que se puede corregir directamente en el prototipo y afecta a la recuperación de errores y a la confirmación comprensible, dos problemas del proceso actual (E5, E10).

---

## 5. Mejora propuesta

**Cambio concreto:** en la Pantalla 4, después de elegir un nuevo horario, mostrar un mensaje de estado con texto: **"Tutoría reprogramada"**.

| | ANTES (v1) | DESPUÉS (v2) |
| --- | --- | --- |
| Pantalla | Pantalla 4: Confirmada y reprogramación | Pantalla 4: Confirmada y reprogramación |
| Comportamiento | La tarjeta de la cita cambia de fecha y hora sin señalar el cambio. | Aparece un mensaje de estado con el resumen "Antes / Ahora" y la acción "Deshacer cambio". |
| Retroalimentación | Implícita (solo cambia el texto de la tarjeta). | Explícita, con texto y no solo color (POUR: perceptible). |
| Recuperación de errores | Para corregir hay que reiniciar el cambio. | Un clic en "Deshacer cambio" restaura el horario anterior (E10). |
| Memoria del usuario | Debe recordar el horario anterior. | El sistema lo muestra (E5). |
| Accesibilidad | Sin anuncio del cambio. | El mensaje se anuncia como estado (`role="status"`) y "Deshacer cambio" es accesible por teclado con foco visible. |

**Conceptos aplicados:** retroalimentación, visibilidad del estado, recuperación de errores, reducción de carga cognitiva, POUR (perceptible, operable y comprensible).

---

## 6. Verificación de la mejora (teórica)

> Esta verificación es **teórica**: se estimó a partir del diseño de la mejora y de los resultados de la v1. No se repitió la prueba con una segunda persona. Los valores de v2 son proyecciones.

| Criterio de verificación | Cómo se comprueba | Resultado esperado en v2 |
| --- | --- | --- |
| El cambio de horario se comunica con texto | Recorrido de la Pantalla 4 tras reprogramar | Se muestra "Tutoría reprogramada" y "Antes → Ahora" |
| El estudiante puede corregir | Pulsar "Deshacer cambio" | Se restablece el horario anterior sin repetir la búsqueda |
| El estudiante no depende de su memoria | Revisar la pantalla sin mirar la conversación previa | Ambos horarios visibles en la misma pantalla |
| Operable con teclado | Tab hasta "Deshacer cambio" y activar con Enter | Foco visible y acción ejecutada |
| No añade pasos al flujo principal | Contar acciones de la tarea T2 | Mismo número de pasos; "Deshacer" es opcional |

### Comparación antes y después

| Indicador | v1 (medido) | v2 (proyección teórica) | Meta |
| --- | --- | --- | --- |
| Tareas completadas sin ayuda | 100 % | 100 % | 100 % |
| Tiempo total | ≈ 2:10 | ≈ 2:00 a 2:10 (sin aumento) | ≤ 3 min |
| Errores en el primer intento | 0 | 0 | ≤ 1 |
| Recuperación de errores | No disponible | Disponible con "Deshacer cambio" | Disponible |
| Certeza sobre el horario vigente | Implícita | Explícita con "Antes / Ahora" | Explícita |
| Satisfacción (1 a 7) | 7 | ≥ 7 | ≥ 5 |

**Interpretación:** la mejora no busca reducir el tiempo, que ya cumple la meta. Busca reforzar la **recuperación de errores** y la **claridad de la confirmación**, dos carencias del proceso por WhatsApp: confirmaciones ambiguas (E3) y fechas olvidadas (E5).

---

## 7. Conclusión

La prueba cruzada con un estudiante de quinto semestre de Ingeniería de Software, paralelo A, mostró que el prototipo v1 cumple las cuatro metas de usabilidad: 100 % de efectividad, tiempo aproximado de 2:10 frente a los 14 minutos del proceso actual (E4), cero errores y satisfacción 7 sobre 7. El participante comprendió el flujo sin explicación previa, lo que respalda el uso de la metáfora de calendario y tarjeta de cita (E9).

El principal punto de mejora fue la falta de retroalimentación explícita al reprogramar. Se propuso un resumen "Antes / Ahora" con opción de deshacer, que responde a E5 y E10 sin añadir pasos. La mejora queda verificada teóricamente y debe confirmarse con una nueva prueba.

## 8. Limitaciones

- La prueba se hizo con **un solo participante**, por lo que los resultados son evidencia cualitativa y no estadística.
- El participante pertenece al mismo curso que el equipo, con posible familiaridad con este tipo de interfaces.
- Se usó **computadora**, aunque el uso previsto es móvil (E1).
- Los tiempos son **aproximados** y no se midieron con una conexión lenta (E8).
- No se evaluó accesibilidad con teclado ni con lector de pantalla (E2).
- La verificación de la mejora fue **teórica**, sin segunda prueba con usuarios.

## 9. Trabajo pendiente

| Pendiente | Descripción | 
| --- | --- |
| Navegación por teclado y atajos | Definir y probar el orden de tabulación, el foco visible y atajos: `Enter` o `Espacio` para seleccionar un horario, `Esc` para cancelar, `Ctrl+Z` o el botón "Deshacer" para revertir. Comprobar que ningún control dependa solo del ratón. |
| Respuestas lentas del servidor | Diseñar estados de carga ("Confirmando tu reserva…"), desactivar el botón mientras se procesa para evitar doble envío, mostrar mensaje si tarda más de lo esperado y permitir reintentar sin perder la selección. | 
| Prueba en móvil | Repetir la prueba en teléfono con otro participante. | 
| Prueba con tecnología de apoyo | Verificar con lector de pantalla y ampliación al 200 %. | 
| Segunda ronda | Probar la v2 con un nuevo participante y actualizar la sección 6 con datos reales. |
