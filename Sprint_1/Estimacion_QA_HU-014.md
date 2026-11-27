# Estimación del esfuerzo de QA · HU-014 Consultar el inventario

| Campo | Valor |
|---|---|
| Responsable | Valeria Usuga |
| Escenarios previstos | 15 (1 básico · 9 alternos · 1 excepción · 4 de calidad) |
| CA cubiertos | 7 de 7 (CA-HU-014-01 a CA-HU-014-07) |
| RNF cubiertos | RNF-004, RNF-005, RNF-008 |
| Puntos de historia | ___ (se acuerdan en equipo con Planning Poker) |

## Desglose de horas

| Actividad | Base del cálculo | Horas | ¿En este Sprint? |
|---|---|:-:|:-:|
| Análisis, criterios, técnicas y escenarios (1.1–1.4) | Fijo | 2 | Sí |
| Plan y matriz de trazabilidad (2.1–2.2) | Fijo | 2 | Sí |
| Datos de prueba (2.3) | Inventario ficticio de 8 equipos + estado inicial | 1 | Sí |
| Casos y scripts (2.4–2.5) | 15 casos × 0,5 h | 7,5 | Sí |
| Ambiente (2.6) | Fijo | 0,5 | Sí |
| Atender revisión por pares (2.7) | Fijo | 1 | Sí |
| **Subtotal diseño** | | **14** | |
| Ejecución | 15 casos × 0,25 h | 3,75 | No (sin ambiente) |
| Reprueba e incidencias (reserva) | Riesgos Media de HU-014 (R-04, R-05) | 1,5 | No |
| Informe | Fijo | 0,75 | No |
| **Total con ejecución futura** | | **20** | |

> Para el Sprint 1 se compromete solo el **subtotal de diseño: 14 h**. Este valor se lleva a `Capacidad_QA.md`.
