# Mapa de riesgos de calidad · Grupo 4

> **BORRADOR – pendiente de validación del equipo.**
> Los riesgos salen de las reglas y criterios de las fichas de HU-014, 015, 016, 017 y 023. La probabilidad y el impacto son una **propuesta inicial** para discutir en equipo.

Severidad = probabilidad × impacto (escala 1–5). **1–6 Baja · 8–12 Media · 15–25 Alta**

| N.º | Riesgo (qué falla → consecuencia) | Prob. | Impacto | Severidad | Prioridad | HU afectadas | Origen en la ficha | Mitigación de QA |
|---|---|:-:|:-:|:-:|---|---|---|---|
| R-01 | Se elimina un equipo que tiene préstamos devueltos → se pierde el historial de asignaciones | 3 | 5 | 15 | Alta | HU-017, HU-023 | HU-017 CA-04, reglas 26–27 | Escenarios separados para préstamo activo, vencido y devuelto; comprobar el historial después del rechazo |
| R-02 | Registrar, editar o eliminar sin el rol requerido porque el servicio solo oculta el botón → cambios no autorizados en el inventario | 3 | 5 | 15 | Alta | HU-015, HU-016, HU-017 | RNF-002 · HU-015 CA-06 · HU-016 CA-08 · HU-017 CA-05 | Probar sin sesión y con cada rol; comparar datos antes y después del rechazo |
| R-03 | Se acepta una serie repetida al registrar o editar → dos equipos con la misma serie | 3 | 4 | 12 | Media | HU-015, HU-016 | HU-015 CA-04 · HU-016 CA-03 | Datos con serie existente; confirmar que el registro anterior se conserva |
| R-04 | Un fallo de consulta se muestra como «sin coincidencias» o «historial vacío» → la persona cree que no hay equipos o préstamos | 3 | 3 | 9 | Media | HU-014, HU-023 | HU-014 CA-05/06 · HU-023 CA-03/04 | Escenarios distintos para vacío y para fallo |
| R-05 | La búsqueda o los filtros combinados muestran equipos que no cumplen o dejan por fuera coincidencias (mayúsculas, serie) → resultados incorrectos | 3 | 3 | 9 | Media | HU-014 | HU-014 CA-02/03, reglas 29–30 | Partición por campo (nombre, marca, serie) y tabla de decisión de filtros |
| R-06 | El historial muestra préstamos de otro dispositivo → información equivocada sobre el equipo | 2 | 4 | 8 | Media | HU-023 | HU-023 CA-02, regla 22 | Datos con varios equipos con préstamos |
| R-07 | Un registro, edición o eliminación aceptada no permanece después de reiniciar el servicio | 2 | 4 | 8 | Media | HU-015, HU-016, HU-017 | RNF-003 | Escenario de calidad de conservación tras reinicio |
| R-08 | Se pierden o se dan por guardados cambios no enviados en la edición | 2 | 3 | 6 | Baja | HU-016 | HU-016 CA-06, regla 37 | Escenario de salida con cambios sin guardar |
| R-09 | Las condiciones de búsqueda no se recuperan al recargar, abrir el enlace o usar Atrás | 3 | 2 | 6 | Baja | HU-014 | HU-014 CA-07 · dependencia RF-027 | Un escenario por cada forma de recuperar la consulta |

> **Para validar en equipo:** ajustar probabilidades e impactos, agregar riesgos que falten y copiar los de cada HU a la sección 10 de su `2.1_Plan_de_pruebas.md`.
