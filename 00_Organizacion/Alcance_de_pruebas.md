# Alcance de las pruebas · Grupo 4

> **BORRADOR – pendiente de validación del equipo.**

## Objetivo de diseño (propuesta)

Diseñar, para cada HU del Grupo 4, un banco de pruebas trazable (CA → escenario → caso → dato → script) que otra persona pueda seguir sin ayuda del autor.

## Dentro del alcance

- **Historias:** HU-014, HU-015, HU-016, HU-017 y HU-023.
- **Fases:** Preparación (1.1–1.4) e Implementación (2.1–2.7) de cada HU.
- **Tipos de prueba:** funcionales de caja negra y no funcionales solo según los RNF que declara cada ficha (ver [Matriz de tipos](Matriz_tipos_de_prueba.md)).
- **Pantallas:** computador y teléfono móvil (RNF-005).
- **Revisión:** las 5 HU del Grupo 5 (HU-018, 019, 020, 021 y 028).

## Fuera del alcance

| Elemento | Razón |
|---|---|
| Ejecución real de los scripts | La guía indica que el diseño no exige una instalación funcional de Device Systems; se deja «No ejecutado» |
| Resultados, capturas o defectos | No se inventan: solo se registran si hay una corrida autorizada |
| Paginación del inventario | HU-014, regla 32: no hace parte de la historia |
| Pruebas de caja blanca y unitarias | Corresponden a desarrollo |
| Rendimiento | Ninguna ficha del grupo define un requisito de rendimiento |
| HU de otros grupos (diseño) | Asignadas a otros equipos |

## Supuestos y restricciones

- Solo datos y cuentas **ficticias**.
- No se inventan URL de servicio, códigos de respuesta ni textos de error que la ficha no especifique.
- Lo que la ficha no aclara se registra como **pregunta al Product Owner** en el [Acta de refinamiento](../Sprint_1/Acta_de_refinamiento.md).
