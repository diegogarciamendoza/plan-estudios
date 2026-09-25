<p align="center">
  <strong>PLAN-ESTUDIOS</strong><br>
  <em>Ruta SOC / Seguridad Defensiva · 12 meses · v3</em><br>
  Repositorio de estudio personal — progreso semanal, notas, labs y entregables.
</p>

---

## 🎯 Objetivo

> En 12 meses, demostrar competencias de SOC L1 con **3 investigaciones reproducibles**, un
> laboratorio funcional, **Security+** si el presupuesto lo permite y **experiencia real de
> postulación/entrevista**.

**Perfil**: 40+ · 20 h/semana · inglés técnico intermedio · base: Linux, reparación, redes, electrónica.

## 🗺️ Ruta (12 meses)

| Fase | Periodo | Contenido | Certificación | Progreso |
|---|---|---|---|---|
| **M1** | Meses 1–2 | Google Cybersecurity + TryHackMe SOC | Google (Coursera) | `█░░░░` **Curso 1/9 ✅** · 4/4 módulos · 90.63% · **Curso 2: 1/4 módulos ✅ 100%** |
| **M2** | Meses 7–8 | Security+ SY0-701 | **Security+** 🎯 | `░░░░░` 0% |
| **M3** | Meses 9–12 | Especialización + CySA+ (opcional) | CySA+/eJPT | `░░░░░` 0% |

📄 [GENERAL.md](GENERAL.md) — el plan completo (12 meses) · 📅 [MES-1-DETALLADO.md](M1-fundamentos/MES-1-DETALLADO.md) · 🧭 [SEMANA-1.md](M1-fundamentos/SEMANA-1.md) · 🎛️ [MODO-CURSERA-INGLES.md](M1-fundamentos/MODO-CURSERA-INGLES.md) · 🃏 [hojas/](hojas/README.md) — hojas de recuperación por módulo

## 📌 Día actual

**▶️ Día 7** (2026-09-24, en curso: **Curso 2 *Play It Safe* · módulo 1 ✅ `Passed · 100%`**; falta el bloque de inglés oral) · Día 6 cerrado: [diario/2026-09-22.md](diario/2026-09-22.md) · **siguiente: módulo 2 *Security frameworks and controls*** (vence **Oct 2**, junto a la *Portfolio Activity: Conduct a security audit*)

> 🗓️ **2026-09-24 (jueves)**: sesión de diseño (**hojas de recuperación por módulo**, [hojas/](hojas/README.md)) **+ Curso 2 · módulo 1** cerrado con `Module 1 challenge` `Passed · Grade: 100%` (captura verificada) · [nota del día](diario/2026-09-24.md) abierta: falta el bloque de inglés y **producir los 8 dominios CISSP de memoria**. El **09-23 no tiene nota**.

> 🎛️ **Modo vigente desde el Día 5: Coursera + inglés** ([detalle](M1-fundamentos/MODO-CURSERA-INGLES.md)). Los labs paralelos (Bandit, bloque Git, Packet Tracer, Messer) quedan **pausados con condición de reactivación** según el curso.

## 📈 Progreso diario (en qué día voy)

_`[x]` hecho · `[ ]` pendiente — marca al cerrar cada día de estudio; el link va a la nota del día._

| Día    | Tema                                              | Estado                                             |
| ------ | ------------------------------------------------- | -------------------------------------------------- |
| **01** | Shell: `pwd ls cd cat less man` | ✅ [nota](diario/2026-09-17.md) |
| 02 | Redes TCP/IP + DNS + Linux self-paced (TryHackMe) | ✅ [nota](diario/2026-09-18.md) · DNS cerrado el 19 |
| 03 | HTTP/TLS + Bandit 2–4 | ✅ [nota](diario/2026-09-19.md) · Bandit hasta la cuenta 8 · handshake explicado |
| 04 | Git + glosario SOC + Coursera mód 2–3 + repaso SRS | ✅ [nota](diario/2026-09-20.md) · challenges 85% y 95% verificados · arrastra: glosario 2/20 |
| 05 | Medición de inglés (EFSET) + reenfoque del plan | ✅ [nota](diario/2026-09-21.md) · EFSET **C1 66** verificado (W 59 · S 48 = producción) · modo **Coursera + inglés** · el curso no avanzó: README y baseline → domingo-flex |
| 06 | Coursera Curso 1 · **módulo 4** + inglés oral | 🔄 [nota](diario/2026-09-22.md) · ✅ **Curso 1 COMPLETO** (90.63% · *Module 4 challenge* **94.44%**, captura verificada) + certificado en el repo · **falta el bloque de inglés** |
| 07 | Curso 2 · **módulo 1 *Security domains*** + diseño de las hojas de recuperación | 🔄 [nota](diario/2026-09-24.md) · ✅ **mód 1/4** (*Module 1 challenge* `Passed · **100%**`, captura verificada) · falta el bloque de inglés y los 8 dominios CISSP de memoria · *(el 09-23 quedó sin nota)* |

_Leyenda: ✅ hecho · 🔄 en curso · ⬜ pendiente_

## 📁 Estructura

```
plan-estudios/
├── README.md            ← este archivo (panel: mapa, progreso, día actual)
├── GENERAL.md           ← plan de 12 meses (referencia, se lee al planear)
├── glosario.md          ← inglés: términos SOC (crece todo el año)
├── vacantes-*.md        ← mercado laboral (referencia)
├── diario/              ← 1 nota por día, TODO el día: YYYY-MM-DD.md
├── hojas/               ← 1 hoja de recuperación por MÓDULO de Coursera (CX-MXX-<slug>)
├── attachments/         ← imágenes/capturas (Obsidian pega aquí: `.obsidian/app.json`)
├── M1-fundamentos/      ← solo lo durable: SEMANA-N, MES-1, tablero, entregables grandes
├── M2-security-plus/    ← meses 7-8
├── M3-especializacion/  ← meses 9-12
└── plantillas/          ← diaria.md + hoja-modulo.md
```

**Regla (KISS):** lo de cada día va en `diario/YYYY-MM-DD.md`, con todo junto (aprendí + práctica + duda). Solo sube al módulo lo que de verdad va a **crecer o reutilizarse** (glosario, scripts, entregables grandes). Si dudas, va al diario — nada de decidir tipos por cada nota.

## 🧭 Cómo lo uso a diario

1. **Nota del día:** `Ctrl+P` → "Periodic Notes: Open daily note" (se crea en `diario/` con la plantilla).
2. **Todo el día ahí**: aprendí + comandos + práctica + duda. 5 min al cerrar el bloque.
3. **Hoja del módulo** ([hojas/](hojas/README.md)): se abre cuando **empieza** un módulo de Coursera y se cierra el día que apruebas su *module challenge*. Se **responde** (respuestas en callout plegado), no se lee.
4. **Tablero semanal** ([tablero.md](M1-fundamentos/tablero.md)): muevo lo hecho a "Hecho" el domingo (o yo lo actualizo).
5. **README**: marco `[x]` en la tabla diaria y enlazo la nota del día.
6. **Sync:** automático cada 30 min con Obsidian abierto (`Ctrl+P` → "Obsidian Git: Commit-and-sync" para forzar; si falla, ver "cómo resolver pull" abajo).

Teclas: `Ctrl+O` abrir rápido · `Ctrl+Shift+F` buscar en todo · `Ctrl+E` leer/editar.

## 🔒 Notas personales

- Este repo es **público** (muestra evidencia de estudio y progreso — suma al CV).
- ⚠️ Nada de credenciales reales ni datos sensibles: cualquier `*bandit*.md` está en `.gitignore`, no se sube.
- Regla de oro: **un commit por día de estudio** — si no está en el repo, no está hecho.

## 🔧 Trouble-shooting del sync (Windows)

- **Pull failed (merge)**: hay cambios locales sin commitear que el pull no puede sobrescribir → `git stash` → `git pull` → `git stash pop`. Si `pop` da `deleted by us`, es un archivo viejo eliminado: descartarlo con `git rm` y `git stash drop`.
- **"Modified" fantasma** (LF↔CRLF, diff vacío): costumbre de Obsidian en Windows; descartar con `git checkout -- <archivo>`.

---
_Actualizado: Día 6 · 2026-09-22 · Semana 1 · ⚠️ el certificado pasó de **8 a 9 cursos** (verificado en coursera.org)_
