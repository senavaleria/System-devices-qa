# Flujo metodológico del proceso de pruebas · HU-XXX [Nombre]

[Portada](README.md) · [Nomenclatura y codificación](00_Nomenclatura.md)

El proceso se organiza en **cuatro fases**. Cada fase recibe insumos, realiza actividades y entrega artefactos que alimentan la siguiente.

## Cadena de trazabilidad

```text
HU-XXX / RF-XXX
   ↓  ___ criterios de aceptación (Dado–Cuando–Entonces) + ___ condiciones de calidad
Escenarios ESC-MOD-FUN-001 … NNN  (básico, alternos, excepciones, calidad)
   ↓
Casos MOD-FUN-001 … NNN  → qué se comprueba
   ↓
Scripts SCR-MOD-FUN-001 … NNN  → cómo se comprueba
   ↓
Ejecución → resultado real → incidencia → reprueba → informe → mejora
```

## Fases, actividades y artefactos

| Fase | Insumos (completar) | Actividades | Artefactos de salida |
|---|---|---|---|
| **1. Preparación** | HU-XXX, reglas RN-___, RNF ___, dependencias ___ | Analizar la historia; descomponer criterios; aclarar vacíos con el PO; elegir tipos y técnicas; generar escenarios | [1.1](01_Preparacion/1.1_Analisis_de_la_HU.md) · [1.2](01_Preparacion/1.2_Criterios_de_aceptacion.md) · [1.3](01_Preparacion/1.3_Tipos_y_tecnicas_de_prueba.md) · [1.4](01_Preparacion/1.4_Escenarios_de_prueba.md) |
| **2. Implementación** | Escenarios, técnicas, preguntas resueltas | Redactar el plan; construir la matriz; preparar datos; redactar casos y scripts; definir el ambiente; revisar por pares | [2.1](02_Implementacion/2.1_Plan_de_pruebas.md) · [2.2](02_Implementacion/2.2_Matriz_de_trazabilidad.md) · [2.3](02_Implementacion/2.3_Datos_de_prueba.md) · [2.4](02_Implementacion/2.4_Casos_de_prueba/00_Indice_de_casos.md) · [2.5](02_Implementacion/2.5_Scripts_de_prueba/_Plantilla_Script.md) · [2.6](02_Implementacion/2.6_Ambiente_de_pruebas.md) · [2.7](02_Implementacion/2.7_Revision_por_pares.md) |
| **3. Ejecución** | Banco revisado, ambiente, versión del producto | Planificar el orden; verificar el entorno; cargar datos; evaluar criterios de entrada; ejecutar y registrar | [3.1](03_Ejecucion/3.1_Preparacion_de_la_ejecucion.md) · [3.2](03_Ejecucion/3.2_Registro_de_ejecucion.md) |
| **4. Evaluación** | Resultados reales, evidencias | Analizar fallos; gestionar incidencias; reprobar; consolidar informe; proponer mejoras | [4.1](04_Evaluacion/4.1_Gestion_de_incidencias.md) · [4.2](04_Evaluacion/4.2_Informe_de_resultados.md) · [4.3](04_Evaluacion/4.3_Plan_de_mejora_continua.md) |

## Puntos de control entre fases

| Paso | Pregunta de control | ¿Cumple? | Acción si no cumple |
|---|---|:-:|---|
| Preparación → Implementación | ¿Cada criterio tiene condiciones observables y las dudas están resueltas o registradas? | ☐ | ___ |
| Implementación → Ejecución | ¿Cada escenario tiene caso, script y datos, y la revisión por pares está cerrada? | ☐ | ___ |
| Ejecución → Evaluación | ¿Todos los casos tienen un estado (Pasó, Falló, Bloqueado, No ejecutado)? | ☐ | ___ |
| Evaluación → Cierre | ¿Las incidencias que impiden cumplir un criterio están verificadas y cerradas? | ☐ | ___ |

## Ubicación del flujo dentro de Scrum

| Evento o artefacto Scrum | Fase de pruebas | Qué se hace con HU-XXX |
|---|---|---|
| Refinamiento del Product Backlog | 1. Preparación | [completar] |
| Sprint Planning | 2. Implementación (plan) | [completar] |
| Durante el Sprint (Daily Scrum) | 2 y 3 | [completar] |
| Definición de Terminado | Criterios de salida | [completar] |
| Sprint Review | 4. Evaluación (informe) | [completar] |
| Sprint Retrospective | 4. Evaluación (mejora) | [completar] |
