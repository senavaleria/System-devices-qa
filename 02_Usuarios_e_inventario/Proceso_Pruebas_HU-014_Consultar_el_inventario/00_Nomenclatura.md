# Nomenclatura y codificación

[Portada](README.md) · [Flujo metodológico](00_Flujo_metodologico.md)

Cada código identifica un solo artefacto y permite seguir la cadena **historia → criterio → escenario → caso → script → resultado → incidencia**.

## 1. Anatomía de un código de prueba

```text
   SCR - MOD - FUN - 001
    │     │     │     └── Consecutivo: tres dígitos, empieza en 001
    │     │     └──────── Funcionalidad (3–4 letras)
    │     └────────────── Módulo (3 letras)
    └──────────────────── Tipo de artefacto
```

## 2. Códigos de los requisitos (vienen de la especificación)

| Prefijo | Significado | Formato |
|---|---|---|
| HU | Historia de usuario | `HU-NNN` |
| RF | Requisito funcional | `RF-NNN` |
| RN | Regla de negocio | `RN-NNN` |
| RNF | Requisito no funcional | `RNF-NNN` |
| CA | Criterio de aceptación | `CA-HU-NNN-NN` |
| CC | Criterio de calidad verificable | `CC-NNN` |

## 3. Códigos del banco de pruebas (los crea el equipo)

| Prefijo | Artefacto | Formato | Regla |
|---|---|---|---|
| ESC | Escenario | `ESC-MOD-FUN-NNN` | Un escenario por condición que cambia el resultado |
| *(sin prefijo)* | Caso de prueba | `MOD-FUN-NNN` | Al menos un caso por escenario |
| SCR | Script | `SCR-MOD-FUN-NNN` | Un script por caso, mismo consecutivo |
| D | Dato de prueba | `D-NNN` o `D-NNNX` | `NNN` = caso; la letra distingue envíos |
| PA | Pregunta abierta al PO | `PA-NN` | Se resuelve en el refinamiento |
| C | Corrida de ejecución | `C-NNN` | Cada ejecución o reprueba es una corrida nueva |
| INC | Incidencia | `INC-MOD-FUN-NNN` | Consecutivo propio |

## 4. Códigos de esta historia (completar)

| Elemento | Valor |
|---|---|
| Módulo (`MOD`) | ___ — [nombre del módulo] |
| Funcionalidad (`FUN`) | ___ — [verbo principal de la historia] |
| Prefijo resultante | `___-___` |
| ¿Se verificó que la combinación no existe? | ☐ Sí |

## 5. Estados

**Artefacto:** Borrador · Revisado · Aprobado · Obsoleto
**Ejecución:** No ejecutado · Pasó · Falló · Bloqueado
**Incidencia:** Nuevo → Abierto → Asignado → Corregido → Verificado → Cerrado (salidas: Rechazado, Diferido, Reabierto)

## 6. Clasificación de escenarios

| Tipo | Significado |
|---|---|
| Básico (*happy path*) | Recorrido principal con datos válidos |
| Alterno | Variante válida del recorrido |
| Excepción (*error path*) | El sistema debe rechazar o informar un error |
| Calidad | Verifica una condición no funcional |

## 7. Nombres de archivos

| Patrón | Ejemplo |
|---|---|
| `<código>.md` por caso o script | `MOD-FUN-001.md`, `SCR-MOD-FUN-001.md` |
| Evidencia | `C-<corrida>_<caso>_paso<N>.png` |

## 8. Reglas de estabilidad

1. No renumerar. 2. No reutilizar códigos retirados (marcar *Obsoleto*). 3. Conservar los códigos oficiales. 4. Relación uno a uno caso–script. 5. Tres dígitos en el consecutivo.
