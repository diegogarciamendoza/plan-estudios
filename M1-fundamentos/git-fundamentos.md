# Bloque Git — fundamentos (M1)

> **Diagnóstico: 2026-09-20 · 4/10** — comandos por necesidad ✅, modelo mental a medias.
> Lo pedí yo (Diego): *"se usar algunos comandos en el día a día pero ha sido un uso completamente superficial; no sabes qué tanto sé de Git en realidad"*.
> **Evidencia del diagnóstico** (respuestas sin consultar nada): working tree ✅ · índice ⚠️ (lo describió como "archivos no trackeados", es un **snapshot de contenido**) · commit ❌ ("guarda todos los cambios" — guarda **solo lo del índice**, demostrado con `git add` → editar → commit: la segunda edición **no** entró) · `commit` de dónde toma ✅ · "qué cambió un commit" ⚠️ (`git log` **lista**; lo que cambió es `git show`) · deshacer ❌ (en blanco) · rama ❌ ("bifurcación del working tree que integro con push" → es un **puntero a un commit**, y lo que integra es **`merge`**).

## Qué se salta (ya lo tiene)

- Cap. 1 de Pro Git: instalación, qué es un control de versiones.
- Comandos básicos: `add` / `commit` / `push` / `pull` / `clone` / `status` los usa a diario (incluso resolvió un conflicto de merge real en el vault).

## Las 3 sesiones (45 min cada una)

| # | Objetivo | Criterio de cierre (medible) | Fuente + práctica |
|---|---|---|---|
| **1** | El **modelo**: worktree · índice · commit | Explicar con un experimento propio por qué `commit` no guarda todos los cambios; y distinguir `git diff` / `--staged` / `HEAD` | Pro Git cap. 2 (`Control de Versiones` → *Fundamentos*) + experimento en repo de prueba |
| **2** | **Historial y deshacer** | Dado un caso ("modifiqué sin commitear", "ya hice `add`", "ya commiteé pero no pusheé"), elegir el comando correcto y decir por qué | Pro Git cap. 2–3 · `git help restore` · `git help show` |
| **3** | **Ramas y merge** ⭐ (hueco principal) | Provocar y **resolver** un conflicto de merge a propósito, explicando qué hace `merge` que `push` no hace | [Learn Git Branching](https://learngitbranching.js.org/) + conflicto real en repo de prueba |

## Glosario mínimo (llenar con TUS palabras al final de cada sesión)

| Término | Qué es | Lo lleno yo |
|---|---|---|
| working tree | | |
| índice / stage | | |
| `HEAD` | | |
| rama (branch) | | |
| `merge` | | |
| `reset` vs `revert` | | |

## Fuentes (verificadas 2026-09-20, HTTP 200)

- [Pro Git v2 en español](https://git-scm.com/book/es/v2) — Chacon & Straub, gratis, en el sitio oficial de Git (fuente primaria).
- [Learn Git Branching](https://learngitbranching.js.org/) — ramas/merge visuales e interactivos.
- [gitglossary](https://git-scm.com/docs/gitglossary) — definiciones oficiales (*index*, *HEAD*, *working tree*).
- [GitHub Skills](https://github.com/skills) — flujo de PRs (no el modelo).
- ⛔ Descartado: *MIT Missing Semester* `/version-control/` → **404**, la ruta cambió.

## Regla de tarjetas para este bloque

Las tarjetas de Git del SRS se crean **al cerrar cada sesión**, no antes: el error de hoy queda documentado aquí, pero no se tarjetea lo que todavía no se trabajó (tarjeta antes de aprender = tarjeta para fallar).

## Huecos a tarjetear (al terminar cada sesión)

- [ ] `commit` guarda **solo el índice** (no el worktree completo).
- [ ] `add` copia **contenido** al índice → lo editado después no entra.
- [ ] rama = **puntero a un commit**; integra `merge`, no `push`.
- [ ] ver **qué cambió** un commit: `git show <commit>` (no `git log`).
- [ ] deshacer: `restore` / `restore --staged` / `reset` vs `revert`.
