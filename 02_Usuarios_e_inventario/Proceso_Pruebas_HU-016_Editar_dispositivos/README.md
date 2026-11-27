# Plantilla del proceso de pruebas · HU-XXX [Nombre de la historia]

**Empieza aquí:** [Flujo metodológico](00_Flujo_metodologico.md) · [Nomenclatura](00_Nomenclatura.md)

> **Cómo usar esta plantilla:** copia la carpeta completa, renómbrala con el código y nombre de tu historia (p. ej., `Proceso_Pruebas_HU-014_Registrar_dispositivo`) y reemplaza los marcadores:
> - `HU-XXX`, `RF-XXX`, `CA-HU-XXX-NN` → códigos oficiales de la historia.
> - `MOD-FUN` → código de módulo y funcionalidad (ver [Nomenclatura](00_Nomenclatura.md)).
> - `[texto entre corchetes]` → contenido que debes redactar.
> - `___` → dato corto por completar.
> Borra estas notas de ayuda (bloques `>`) cuando termines.

| Control del banco | Valor |
|---|---|
| Proyecto | ___ |
| Historia | HU-XXX [Nombre] · RF-XXX |
| Versión del banco | ___ |
| Versión del producto | ___ |
| Responsable de elaboración | ___ |
| Responsable de revisión | ___ |
| Última actualización | __/__/____ |
| Estado del artefacto | Borrador / Revisado / Aprobado / Obsoleto |
| Estado de ejecución | No ejecutado / En ejecución / Ejecutado |

## Organización del directorio

```text
Proceso_Pruebas_HU-XXX/
├── README.md
├── 00_Flujo_metodologico.md
├── 00_Nomenclatura.md
├── 01_Preparacion/
│   ├── 1.1_Analisis_de_la_HU.md
│   ├── 1.2_Criterios_de_aceptacion.md
│   ├── 1.3_Tipos_y_tecnicas_de_prueba.md
│   └── 1.4_Escenarios_de_prueba.md
├── 02_Implementacion/
│   ├── 2.1_Plan_de_pruebas.md
│   ├── 2.2_Matriz_de_trazabilidad.md
│   ├── 2.3_Datos_de_prueba.md  (+ .csv)
│   ├── 2.4_Casos_de_prueba/      00_Indice_de_casos.md · _Plantilla_Caso.md
│   ├── 2.5_Scripts_de_prueba/    _Plantilla_Script.md
│   ├── 2.6_Ambiente_de_pruebas.md
│   └── 2.7_Revision_por_pares.md
├── 03_Ejecucion/
│   ├── 3.1_Preparacion_de_la_ejecucion.md
│   └── 3.2_Registro_de_ejecucion.md
└── 04_Evaluacion/
    ├── 4.1_Gestion_de_incidencias.md
    ├── 4.2_Informe_de_resultados.md
    └── 4.3_Plan_de_mejora_continua.md
```

## Convención de identificadores

| Artefacto | Formato | Ejemplo con tu historia |
|---|---|---|
| Escenario | `ESC-MOD-FUN-NNN` | ___ |
| Caso | `MOD-FUN-NNN` | ___ |
| Script | `SCR-MOD-FUN-NNN` | ___ |
| Dato | `D-NNN[A-D]` | ___ |
| Incidencia | `INC-MOD-FUN-NNN` | ___ |

## Estado de los artefactos

Borrador → Revisado (tras 2.7) → Aprobado (aceptado por el PO) → Obsoleto (si la historia cambia).
