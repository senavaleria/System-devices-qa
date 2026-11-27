# Guía del equipo · Cómo subir tu HU

La nota es **individual**: cada persona trabaja **solo su HU**, en **su propia rama** y con **su propia Pull Request (PR)**. Así el instructor ve qué hizo cada quien.

| Integrante | HU | Rama | Carpeta |
|---|---|---|---|
| Valeria Usuga | HU-014 | `qa/hu-014` | `02_Usuarios_e_inventario/Proceso_Pruebas_HU-014_Consultar_el_inventario/` |
| Juan David Bastidas | HU-015 | `qa/hu-015` | `02_Usuarios_e_inventario/Proceso_Pruebas_HU-015_Registrar_dispositivos/` |
| Yhojan Caro | HU-016 | `qa/hu-016` | `02_Usuarios_e_inventario/Proceso_Pruebas_HU-016_Editar_dispositivos/` |
| Yhojan Caro | HU-017 | `qa/hu-017` | `02_Usuarios_e_inventario/Proceso_Pruebas_HU-017_Eliminar_dispositivos_sin_historial/` |
| Mariana Suarez | HU-023 | `qa/hu-023` | `02_Usuarios_e_inventario/Proceso_Pruebas_HU-023_Consultar_el_historial_de_un_dispositivo/` |

> 💡 **Analogía:** `main` es el cuaderno limpio del equipo. Tu rama es una **fotocopia** donde escribes tranquila. La PR es pedir: «revisen mi fotocopia y, si está bien, pásenla al cuaderno».

En los comandos, cambia `0XX` por el número de tu HU (por ejemplo `015`).

---

## Paso 1 · Aceptar la invitación

1. Abre el correo de GitHub «invited you to collaborate» (o entra a <https://github.com/notifications>).
2. Haz clic en **Accept invitation**.

## Paso 2 · Clonar el repositorio (una sola vez)

Abre **Git Bash** en la carpeta donde quieras guardarlo:

```bash
git clone https://github.com/USUARIO-DE-VALERIA/System-devices-qa.git
cd System-devices-qa
```

| Comando | Qué hace |
|---|---|
| `git clone <url>` | Descarga una copia del repositorio a tu computador |
| `cd System-devices-qa` | Entra a la carpeta que se descargó |

## Paso 3 · Crear TU rama

```bash
git switch main
git pull
git switch -c qa/hu-0XX
```

| Comando | Qué hace |
|---|---|
| `git switch main` | Se para en la rama principal |
| `git pull` | Trae los últimos cambios de GitHub |
| `git switch -c qa/hu-0XX` | Crea tu rama y te cambia a ella (`-c` = crear) |

Comprueba que estás en tu rama: `git branch` (tu rama aparece con `*`).

> Si tienes dos HU (Yhojan): haz la primera completa (pasos 3 a 7), luego vuelve al paso 3 con la segunda. **Dos HU = dos ramas = dos PR.**

## Paso 4 · Trabajar SOLO en tu carpeta

✅ Puedes modificar:

| Archivo | Qué haces |
|---|---|
| Tu carpeta `Proceso_Pruebas_HU-0XX_.../` | Llenas la plantilla de 1.1 a 2.6 (2.7, 03 y 04 quedan con la plantilla) |
| `Sprint_1/Estimacion_QA_HU-0XX.md` | **Lo creas tú.** Copia el de HU-014 como modelo y pon tus números |
| `Sprint_1/Acta_de_refinamiento.md` | Escribes tus preguntas **solo en la sección de tu HU** |
| `Sprint_1/Capacidad_QA.md` | Llenas **solo tu fila** con tus horas reales |

Para copiar la estimación como modelo:

```bash
cp Sprint_1/Estimacion_QA_HU-014.md Sprint_1/Estimacion_QA_HU-0XX.md
```

(`cp` = copiar: primero el archivo original, luego el nombre nuevo.)

## Paso 5 · Guardar tu trabajo (commit) y subirlo (push)

```bash
git status
git add .
git commit -m "HU-0XX: diseño de pruebas (preparación e implementación)"
git push -u origin qa/hu-0XX
```

| Comando | Qué hace |
|---|---|
| `git status` | Muestra qué archivos cambiaste. **Revisa que sean solo los tuyos** |
| `git add .` | Prepara todos tus cambios para guardarlos |
| `git commit -m "..."` | Guarda una «foto» de tus cambios con un mensaje |
| `git push -u origin qa/hu-0XX` | Sube tu rama a GitHub (`-u` la deja conectada para la próxima vez) |

Puedes hacer varios commits mientras avanzas. Después del primero, basta con `git push`.

## Paso 6 · Abrir tu Pull Request hacia `main`

1. En GitHub verás un aviso amarillo **Compare & pull request**. Haz clic.
2. Revisa: **base: `main`** ← **compare: `qa/hu-0XX`**.
3. Título: `[HU-0XX] Diseñar pruebas: <nombre de la HU>`
4. Descripción (copia y completa):

```markdown
## HU-0XX <nombre>

- Issue: #___
- Carpeta: 02_Usuarios_e_inventario/Proceso_Pruebas_HU-0XX_<nombre>/
- Matriz: 02_Usuarios_e_inventario/Proceso_Pruebas_HU-0XX_<nombre>/02_Implementacion/2.2_Matriz_de_trazabilidad.md
- CA cubiertos: CA-HU-0XX-01 … CA-HU-0XX-NN (N de N)
- RNF cubiertos: ___
- Estado de ejecución: No ejecutado

Revisión solicitada a: @usuario-del-revisor (Grupo 3)
```

5. En **Reviewers**, agrega a la persona que designe el Grupo 3.
6. Haz clic en **Create pull request**.
7. En el Project, mueve tu tarea a **En revisión**.

> ⛔ **No hagas Merge tú mismo.** Se fusiona cuando el Grupo 3 la apruebe.

## Paso 7 · Si te piden cambios

Corrige en tu misma rama y vuelve a subir:

```bash
git add .
git commit -m "HU-0XX: corrige observación de revisión"
git push
```

La PR se actualiza sola. Anota la observación y su resolución en tu `2.7_Revision_por_pares.md`.

## Si GitHub dice que hay conflicto

Pasa si alguien cambió las mismas líneas del acta o de la capacidad antes que tú.

```bash
git switch qa/hu-0XX
git pull origin main
```

(`git pull origin main` trae a tu rama lo último de `main`.) Abre el archivo marcado, conserva **tu** sección y la de tus compañeros, borra las líneas `<<<<<<<`, `=======`, `>>>>>>>` y luego haz `git add .`, `git commit` y `git push`. Si te enredas, avísale a Valeria antes de borrar nada.

---

## ⛔ Lo que NO se debe hacer

| No | Por qué |
|---|---|
| Tocar la carpeta de la HU de otra persona | La nota es individual; tu PR debe mostrar solo tu trabajo |
| Hacer `push` directo a `main` | Todo entra por PR revisada |
| Subir datos reales (Excel, cédulas, notas, correos o contraseñas reales) | Lo prohíbe la guía; solo datos ficticios |
| Inventar URL, códigos de respuesta o textos de error | Si la ficha no lo dice, va como pregunta al PO en el acta |
| Marcar resultados como «Pasó» | No hay ejecución: se deja **No ejecutado** |
| Borrar archivos de la plantilla | Las carpetas 03 y 04 se conservan para después |
