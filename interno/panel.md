# Panel interno

**Esto no es la vitrina.** El [README](../README.md) de la raíz está escrito para quien llega de
fuera; aquí está el taller: día actual, tabla de días, cómo uso el vault y las notas de
sincronización. También es donde van las anotaciones operativas del asistente (en las notas diarias
antiguas esas anotaciones siguen dentro como registro histórico).

## Día actual

**▶️ Día 11** (2026-10-08: **arranque del Curso 4 *Tools of the Trade: Linux and SQL***) ·
Último día cerrado: [diario/2026-10-07.md](../diario/2026-10-07.md) — **Curso 3 completo** (`Grade: 98.81%`,
certificado ✅). Quedan abiertos: las **hojas del Curso 3 sin responder** (C03-M01/M02/M03/M04) y la
*portfolio activity* NIST por reformatear.

> ⚠️ **Decisión pendiente para el 10-08:** con el **Curso 4** vencen las condiciones de reactivación de
> **Bandit 9+ / TryHackMe Linux Fundamentals / bloque Git** ([[MODO-CURSERA-INGLES]]). Se decide al
> arrancar el bloque — no antes.

> **Modo vigente desde el Día 5**: Coursera + inglés ([detalle](../M1-fundamentos/MODO-CURSERA-INGLES.md)).
> Los labs paralelos (Bandit, bloque Git, Packet Tracer, Messer) quedan pausados con condición de
> reactivación **atada al curso que los cubre**; las prácticas de redes se re-decidieron el **2026-10-07**
> (siguen pausadas: Messer → prep de Security+, Packet Tracer → fase 2).

## Días de estudio

Del **17 al 30 de septiembre** (14 días): **9 con nota** y **5 sin nota — 23, 25, 27, 28 y 29**.
Los días **10-01 y 10-02 no hubo bloque de estudio del curso** (fueron de investigación y planificación):
quedan **sin nota y sin número de día** — el Curso 3 no arrancó hasta el **10-03**.
Los días **10-04, 10-05 y 10-06** también fueron **pausa real** (declarado el 2026-10-07): sin nota y sin
número de día; el bloque se retoma el **10-07**.
No se renumera ningún día: la numeración `Día N` se asigna al **cerrar** el bloque de estudio.

| Día | Fecha | Tema | Nota |
|---|---|---|---|
| 01 | 09-17 | Shell: `pwd ls cd cat less man` | [2026-09-17](../diario/2026-09-17.md) |
| 02 | 09-18 | Redes TCP/IP + DNS + Linux self-paced (TryHackMe) | [2026-09-18](../diario/2026-09-18.md) |
| 03 | 09-19 | HTTP/TLS + Bandit 0→8 | [2026-09-19](../diario/2026-09-19.md) |
| 04 | 09-20 | Git + glosario SOC + Coursera mód. 2–3 + repaso SRS | [2026-09-20](../diario/2026-09-20.md) |
| 05 | 09-21 | Medición de inglés (EFSET) + reenfoque del plan | [2026-09-21](../diario/2026-09-21.md) |
| 06 | 09-22 | Coursera Curso 1 · módulo 4 → **Curso 1 completo (90.63%)** | [2026-09-22](../diario/2026-09-22.md) |
| 07 | 09-24 | Curso 2 · módulo 1 *Security domains* (100%) + diseño de las hojas | [2026-09-24](../diario/2026-09-24.md) |
| — | 09-26 | Repaso SRS medido (18/20) + decisión memoria-vs-consulta | [2026-09-26](../diario/2026-09-26.md) |
| 08 | 09-30 | Curso 2 · módulos 2–4 → **Curso 2 completo (98.51%)** ✅ verificado | [2026-09-30](../diario/2026-09-30.md) |
| 09 | 10-03 | **Curso 3 · arranque** (redes y seguridad de red) + M1–M2 cerrados (🟡 declarado) | [2026-10-03](../diario/2026-10-03.md) |
| 10 | 10-07 | Curso 3 · módulos 3 y 4 → **Curso 3 completo (98.81%)** ✅ verificado + SRS oral | [2026-10-07](../diario/2026-10-07.md) |

## Cómo lo uso a diario

1. **Nota del día:** `Ctrl+P` → *Periodic Notes: Open daily note* (se crea en `diario/`).
   Plantilla ligera: [`plantillas/diaria-ligera.md`](../plantillas/diaria-ligera.md).
2. **Al cerrar cada módulo** de un curso: se llena su **hoja de repaso** en `repaso/` y se actualiza
   el **tracker del curso** en `cursos/`.
3. **Tablero semanal:** [`M1-fundamentos/tablero.md`](../M1-fundamentos/tablero.md) (kanban).
4. **README:** solo se toca cuando cambia algo **verificado** de la vitrina.
5. **Sync:** automático cada ~30 min con Obsidian abierto (`Ctrl+P` → *Obsidian Git:
   Commit-and-sync* para forzar).

Teclas: `Ctrl+O` abrir rápido · `Ctrl+Shift+F` buscar en todo · `Ctrl+E` leer/editar.

## Sincronización (Windows) — troubleshooting

- **Pull failed (merge)**: hay cambios locales sin commitear que el pull no puede sobrescribir →
  `git stash` → `git pull` → `git stash pop`. Si `pop` da `deleted by us`, es un archivo viejo
  eliminado: descartarlo con `git rm` y `git stash drop`.
- **"Modified" fantasma** (LF↔CRLF, diff vacío): costumbre de Obsidian en Windows; descartar con
  `git checkout -- <archivo>`. Ya mitigado con el `.gitattributes` (`* text=auto eol=lf`).
- **Obsidian reformatea las tablas** al guardar: produce diffs de alineación sin cambio de
  contenido. No es un conflicto.

## Reglas de oro del repo

- Es **público**: nada de credenciales ni datos sensibles. Cualquier `*bandit*.md` está en
  `.gitignore`.
- **Lo que no está en el repo no está hecho** — pero un commit por día de estudio, no commits
  artificiales para pintar el gráfico de contribuciones.
- El contenido de Coursera (transcripciones, lecturas, quizzes) **nunca** entra al repo.
