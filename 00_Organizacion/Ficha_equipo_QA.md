# Ficha del equipo de QA

| Campo | Valor |
|---|---|
| Proyecto | Device Systems · repositorio `System-devices-qa` |
| Equipo | QA Grupo 4 · Inventario e historial de dispositivos |
| Módulo asignado | 02 · Usuarios e inventario (parte de inventario e historial de dispositivos) |
| HU asignadas | HU-014, HU-015, HU-016, HU-017, HU-023 |
| Product Owner de referencia | Instructor Carlos Navia |
| Líder de pruebas | Valeria Usuga (según la asignación de grupos) |
| Scrum Master | Mariana Suarez |
| Duración del Sprint | ___ (por acordar en equipo) |
| Grupo que revisa nuestras HU | Grupo 3 |
| Grupo cuyas HU revisamos | Grupo 5 · Operación de préstamos y errores |

## Roles del equipo

> En Scrum, QA es parte del equipo de desarrollo: estos roles organizan el trabajo, no crean jerarquías (Tema 7). Una persona puede tener varios roles, salvo ser autora y revisora del mismo artefacto (Tema 6).

| Rol | Persona | Responsabilidades | Reemplazo |
|---|---|---|---|
| Líder de pruebas | Valeria Usuga | Coordinar con el PO; consolidar acta, capacidad y Sprint Backlog; administrar el repositorio y el Project; velar por la DoR y la DoD | Juan David Bastidas |
| Scrum Master | Mariana Suarez | Facilitar Daily, Planning, Review y Retrospectiva; registrar bloqueos en el Project y buscar quién los resuelve | Yhojan Caro |
| Analista y tester de cada HU | Cada responsable de HU (tabla siguiente) | Análisis, escenarios, matriz, datos, casos y scripts de su HU (1.1–2.6) | Otro integrante del equipo |
| Revisor par de nuestras HU | Persona designada por el Grupo 3 | Revisar cada HU antes de fusionarla y registrar en 2.7 y en la PR | Otra persona del Grupo 3 |

## Diseño de HU (autoría individual)

| Integrante | HU que diseña | Rama | PR |
|---|---|---|---|
| Valeria Usuga | HU-014 | `qa/hu-014` | 1 |
| Juan David Bastidas | HU-015 | `qa/hu-015` | 1 |
| Yhojan Caro | HU-016 · HU-017 | `qa/hu-016` · `qa/hu-017` | 2 |
| Mariana Suarez | HU-023 | `qa/hu-023` | 1 |

## Revisión de las HU del Grupo 5 (propuesta)

Cada integrante revisa al menos una HU del Grupo 5. Nadie revisa una HU de la que es autor.

| Integrante | HU del Grupo 5 que revisa |
|---|---|
| Valeria Usuga | HU-018 Registrar un préstamo |
| Juan David Bastidas | HU-019 Consultar el panel de préstamos · HU-028 Comunicar errores de operación |
| Yhojan Caro | HU-020 Registrar la devolución de un dispositivo |
| Mariana Suarez | HU-021 Marcar un préstamo como vencido |

> Yhojan revisa una sola HU porque diseña dos.

## Herramientas

| Herramienta | Uso |
|---|---|
| GitHub (repositorio) | Ramas `qa/hu-0XX`, Pull Requests y revisión |
| GitHub Projects | Tablero Pendiente → En curso → En revisión → Hecho |
| Editor de Markdown y CSV (VS Code u otro) | Redactar los archivos del banco de pruebas |
| Git Bash | Clonar, crear ramas, commit y push |
