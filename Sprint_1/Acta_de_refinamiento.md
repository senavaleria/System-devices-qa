# Acta de refinamiento · Sprint 1 · Grupo 4

> **BORRADOR – pendiente de validación del equipo.** Contiene solo las preguntas de HU-014. Cada integrante agrega las de su HU en su sección.

| Campo | Valor |
|---|---|
| Fecha | __/__/____ |
| Participantes | PO: Instructor Carlos Navia · QA: Valeria Usuga, Juan David Bastidas, Yhojan Caro, Mariana Suarez |
| HU revisadas | HU-014, HU-015, HU-016, HU-017, HU-023 |

> Regla: una pregunta no detiene el diseño. Se trabaja con la **interpretación provisional** y se ajusta cuando el PO responda. No se convierte una suposición en requisito.

---

## HU-014 Consultar el inventario · Valeria Usuga

| ID | Pregunta para el PO | Interpretación provisional | CA afectados | Respuesta del PO | Cambio en escenarios |
|---|---|---|---|---|---|
| PA-01 | La ficha dice que la búsqueda se hace «cuando la persona deja de escribir». ¿Cuánto tiempo sin escribir cuenta como «dejar de escribir»? | Se comprueba que una escritura continua genera **una sola** consulta al terminar; no se mide un tiempo exacto. | CA-HU-014-04 | Pendiente | — |
| PA-02 | ¿Qué opciones tiene el filtro de disponibilidad (por ejemplo, disponible / no disponible)? | Se usan dos valores: disponible y no disponible. | CA-HU-014-03 | Pendiente | — |
| PA-03 | ¿Las opciones del filtro de tipo son los seis tipos admitidos en HU-015 (portátil, tableta, proyector, cámara, enrutador, monitor)? | Sí, se usan esos seis tipos. | CA-HU-014-03 | Pendiente | — |
| PA-04 | ¿Qué datos debe mostrar cada tarjeta además de la disponibilidad? | Nombre, marca, tipo, serie y disponibilidad. | CA-HU-014-01, CA-HU-014-03 | Pendiente | — |
| PA-05 | La búsqueda no distingue mayúsculas. ¿Tampoco distingue tildes (por ejemplo «cámara» y «camara»)? | Solo se prueba mayúsculas/minúsculas; las tildes quedan fuera hasta que el PO responda. | CA-HU-014-02 | Pendiente | — |
| PA-06 | En «Dependencias» la ficha nombra RNF-005, pero en «Condiciones de calidad» aplica RNF-004, RNF-005 y RNF-008. ¿Se prueban los tres? | Sí, se prueban los tres que aparecen en «Condiciones de calidad». | Escenarios de calidad | Pendiente | — |
| PA-07 | Si el texto de búsqueda queda vacío, ¿se muestran de nuevo todos los equipos que cumplen los filtros? | Fuera de alcance hasta la respuesta; no se diseña caso. | — | Pendiente | — |

---

## HU-015 Registrar dispositivos · Juan David Bastidas

| ID | Pregunta para el PO | Interpretación provisional | CA afectados | Respuesta del PO | Cambio en escenarios |
|---|---|---|---|---|---|
| PA-01 | | | | | |

## HU-016 Editar dispositivos · Yhojan Caro

| ID | Pregunta para el PO | Interpretación provisional | CA afectados | Respuesta del PO | Cambio en escenarios |
|---|---|---|---|---|---|
| PA-01 | | | | | |

## HU-017 Eliminar dispositivos sin historial · Yhojan Caro

| ID | Pregunta para el PO | Interpretación provisional | CA afectados | Respuesta del PO | Cambio en escenarios |
|---|---|---|---|---|---|
| PA-01 | | | | | |

## HU-023 Consultar el historial de un dispositivo · Mariana Suarez

| ID | Pregunta para el PO | Interpretación provisional | CA afectados | Respuesta del PO | Cambio en escenarios |
|---|---|---|---|---|---|
| PA-01 | | | | | |

---

## Escenarios acordados

| HU | Total | Agregados | Eliminados |
|---|:-:|:-:|:-:|
| HU-014 | 15 (propuesta) | — | — |
| HU-015 | | | |
| HU-016 | | | |
| HU-017 | | | |
| HU-023 | | | |

## Acuerdos y pendientes

| N.º | Acuerdo o pendiente | Responsable | Fecha |
|---|---|---|---|
| 1 | Llevar las preguntas PA al Product Owner y anotar sus respuestas | Cada responsable de HU | |
