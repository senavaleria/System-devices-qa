# Matriz de tipos de prueba · Módulo 02 · Inventario e historial de dispositivos

> **BORRADOR – pendiente de validación del equipo.**
> Basado en las fichas de las 5 HU y en las condiciones de calidad (RNF) que cada ficha declara.

## Tipo de acceso por HU

| HU | Pantalla / servicio | Acceso según la ficha |
|---|---|---|
| HU-014 Consultar el inventario | Pantalla Inventario (tarjetas, búsqueda y filtros) | **Pública**, con o sin sesión |
| HU-015 Registrar dispositivos | Formulario de dispositivo + servicio | **Restringida**: soporte o administrador |
| HU-016 Editar dispositivos | Mismo formulario de registro + servicio | **Restringida**: soporte o administrador |
| HU-017 Eliminar dispositivos sin historial | Acción Eliminar con diálogo de confirmación + servicio | **Restringida**: solo administrador |
| HU-023 Consultar el historial de un dispositivo | Historial desde el inventario o pantalla relacionada | **Pública**, también para visitantes |

## Tipos de prueba por HU

✅ aplica · ➖ no aplica en esta evidencia

| HU | Funcional (caja negra) | Interfaz / usabilidad | Seguridad (permisos) | Datos / persistencia | API / servicio | Rendimiento | Automatización | Justificación |
|---|:-:|:-:|:-:|:-:|:-:|:-:|:-:|---|
| HU-014 | ✅ | ✅ RNF-004, RNF-005 | ➖ | ➖ | ✅ RNF-008 | ➖ | ➖ | Consulta pública; la ficha pide teclado, pantallas y trazas de respuesta (RNF-004, 005, 008) |
| HU-015 | ✅ | ✅ RNF-004, RNF-005 | ✅ RNF-002 | ✅ RNF-003 | ✅ | ➖ | ➖ | Operación restringida que crea datos |
| HU-016 | ✅ | ✅ RNF-004, RNF-005 | ✅ RNF-002 | ✅ RNF-003 | ✅ | ➖ | ➖ | Operación restringida que modifica datos |
| HU-017 | ✅ | ✅ RNF-004 (foco del diálogo), RNF-005 | ✅ RNF-002 | ✅ RNF-003 | ✅ | ➖ | ➖ | Operación restringida que elimina datos; protege el historial |
| HU-023 | ✅ | ✅ RNF-005, RNF-007 | ➖ | ✅ RNF-003 | ➖ | ➖ | ➖ | Consulta pública de historial con fechas |

> Los RNF de cada fila son los que lista **cada ficha**. No se asignan los ocho RNF a todas las HU.

## Técnicas sugeridas (cada responsable decide y justifica en su 1.3)

| Técnica | Cuándo sirve en este módulo |
|---|---|
| Partición de equivalencia | Campos y tipos admitidos (HU-015, 016), campos de búsqueda (HU-014) |
| Tabla de decisión | Varias condiciones definen el resultado: filtros combinados (HU-014), rol + historial (HU-017) |
| Transición de estados | Equipo disponible / con préstamo / con historial (HU-017, HU-023) |
| Valores límite | Solo si la ficha define un límite numérico |
