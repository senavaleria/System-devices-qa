# System-devices-qa · Grupo 4 · Inventario e historial de dispositivos

Repositorio de diseño de pruebas por historia de usuario del proyecto **Device Systems** (sistema de préstamo de dispositivos).

| Dato | Valor |
|---|---|
| Programa | ADSO · SENA · Ficha 3229209 |
| Competencia | 220501096 · Pruebas de Software y SCRUM |
| Evidencia | GA-220501096-05-EV05 – Diseño de pruebas por historia de usuario con Scrum |
| Instructor (Product Owner) | Carlos Navia |
| Equipo | Grupo 4 · Inventario e historial de dispositivos |
| Grupo revisor de nuestras HU | Grupo 3 |
| Grupo que revisamos | Grupo 5 |
| GitHub Project | Pendiente |

> ⚠️ Solo se usan **datos y cuentas ficticias**. No se publican el Excel, identificaciones, notas, credenciales ni datos reales.

## Índice de historias de usuario

| HU | Nombre | Módulo de origen | Responsable | Revisor (Grupo 3) | Carpeta | Issue |
|---|---|---|---|---|---|---|
| HU-014 | Consultar el inventario | 02 · Usuarios e inventario | Valeria Usuga | Pendiente | [Abrir](02_Usuarios_e_inventario/Proceso_Pruebas_HU-014_Consultar_el_inventario/) | Pendiente |
| HU-015 | Registrar dispositivos | 02 · Usuarios e inventario | Juan David Bastidas | Pendiente | [Abrir](02_Usuarios_e_inventario/Proceso_Pruebas_HU-015_Registrar_dispositivos/) | Pendiente |
| HU-016 | Editar dispositivos | 02 · Usuarios e inventario | Yhojan Caro | Pendiente | [Abrir](02_Usuarios_e_inventario/Proceso_Pruebas_HU-016_Editar_dispositivos/) | Pendiente |
| HU-017 | Eliminar dispositivos sin historial | 02 · Usuarios e inventario | Yhojan Caro | Pendiente | [Abrir](02_Usuarios_e_inventario/Proceso_Pruebas_HU-017_Eliminar_dispositivos_sin_historial/) | Pendiente |
| HU-023 | Consultar el historial de un dispositivo | 02 · Usuarios e inventario | Mariana Suarez | Pendiente | [Abrir](02_Usuarios_e_inventario/Proceso_Pruebas_HU-023_Consultar_el_historial_de_un_dispositivo/) | Pendiente |

## Organización y Sprint

| Carpeta | Contenido |
|---|---|
| [00_Organizacion](00_Organizacion/) | [Ficha del equipo](00_Organizacion/Ficha_equipo_QA.md) · [Asignación de HU](00_Organizacion/Matriz_asignacion_HU.md) · [Riesgos](00_Organizacion/Mapa_de_riesgos.md) · [Tipos de prueba](00_Organizacion/Matriz_tipos_de_prueba.md) · [Alcance](00_Organizacion/Alcance_de_pruebas.md) · [DoR](00_Organizacion/DoR.md) · [DoD](00_Organizacion/DoD.md) |
| [Sprint_1](Sprint_1/) | [Acta de refinamiento](Sprint_1/Acta_de_refinamiento.md) · [Estimación HU-014](Sprint_1/Estimacion_QA_HU-014.md) · [Capacidad](Sprint_1/Capacidad_QA.md) · [Sprint Backlog](Sprint_1/Sprint_Backlog_QA.md) |
| [02_Usuarios_e_inventario](02_Usuarios_e_inventario/) | Una carpeta por HU, copiada de `Plantilla_Proceso_Pruebas_HU-XXX` |

## Cómo trabajar en este repositorio

Lee primero la [Guía del equipo](GUIA_EQUIPO.md): cada integrante trabaja en **su propia rama** (`qa/hu-0XX`), solo dentro de la carpeta de su HU, y entrega con **su propia Pull Request**.

## Estructura

```text
System-devices-qa/
├── README.md
├── GUIA_EQUIPO.md
├── 00_Organizacion/
│   ├── Ficha_equipo_QA.md
│   ├── Matriz_asignacion_HU.md
│   ├── Mapa_de_riesgos.md
│   ├── Matriz_tipos_de_prueba.md
│   ├── Alcance_de_pruebas.md
│   ├── DoR.md
│   └── DoD.md
├── Sprint_1/
│   ├── Acta_de_refinamiento.md
│   ├── Estimacion_QA_HU-014.md
│   ├── Capacidad_QA.md
│   └── Sprint_Backlog_QA.md
└── 02_Usuarios_e_inventario/
    ├── Proceso_Pruebas_HU-014_Consultar_el_inventario/
    ├── Proceso_Pruebas_HU-015_Registrar_dispositivos/
    ├── Proceso_Pruebas_HU-016_Editar_dispositivos/
    ├── Proceso_Pruebas_HU-017_Eliminar_dispositivos_sin_historial/
    └── Proceso_Pruebas_HU-023_Consultar_el_historial_de_un_dispositivo/
```
