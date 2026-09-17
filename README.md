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
| **M1** | Meses 1–2 | Google Cybersecurity + TryHackMe SOC | Google (Coursera) | `██░░░` ~5% |
| **M2** | Meses 7–8 | Security+ SY0-701 | **Security+** 🎯 | `░░░░░` 0% |
| **M3** | Meses 9–12 | Especialización + CySA+ (opcional) | CySA+/eJPT | `░░░░░` 0% |

📄 [GENERAL.md](GENERAL.md) — plan completo · 📅 [MES-1-DETALLADO.md](M1-fundamentos/MES-1-DETALLADO.md) · 🧭 [SEMANA-1.md](M1-fundamentos/SEMANA-1.md)
📋 [Tablero](M1-fundamentos/tablero.md)

## 📌 Día actual

**▶️ Día 1** · `diario/2026-09-17` → [abrirlo](diario/2026-09-17.md)

## 📈 Progreso diario (en qué día voy)

_`[x]` hecho · `[ ]` pendiente — marca cada día al cerrar el bloque._

| Día | Tema | Nota lab | Nota tema | Estado |
|---|---|---|---|---|
| **01** | Shell: `pwd ls cd cat less man` | [dia01-lab-shell](M1-fundamentos/dia01-lab-shell.md) | [dia01-tema-shell](M1-fundamentos/dia01-tema-shell.md) | ✅ |
| 02 | Redes TCP/IP + DNS + `touch mkdir cp mv rm` | — | — | ⬜ |
| 03 | HTTP/TLS + Bandit 2–4 | — | — | ⬜ |
| 04 | Git + Bandit 5 | — | — | ⬜ |
| 05 | Messer Network + README | — | — | ⬜ |
| 06 | Inglés + glosario SOC | — | — | ⬜ |

_Leyenda: ✅ hecho · 🔄 en curso · ⬜ pendiente_

## 📁 Estructura

```
plan-estudios/
├── README.md             ← este archivo (panel: mapa, progreso, día actual, últimas notas)
├── GENERAL.md            ← plan de 12 meses (el mapa)
├── glosario.md           ← inglés: términos SOC (crece todo el año)
├── vacantes-*.md         ← mercado laboral (referencia)
├── diario/               ← crónica por día: YYYY-MM-DD.md (por FECHA)
├── M1-fundamentos/       ← fase actual: diaNN-*, MES-1, SEMANA-N, tablero
├── M2-security-plus/     ← meses 7-8
├── M3-especializacion/   ← meses 9-12
└── plantillas/           ← diaria.md (nota del día) · tema.md (nota de estudio)
```

**Convención de nombres** (en el módulo): `dia<NN>-<tipo>-<slug>.md`
- `dia01-lab-shell.md` → práctica/ejercicio resuelto (evidencia)
- `dia01-tema-shell.md` → concepto durable (plantilla `tema.md`)
- `diaNN-apunte-*.md` → cualquier otra cosa
- El `diario/` usa la fecha en el nombre; el día del plan va en su frontmatter (`dia_plan`).

**Regla:** dentro de un módulo todo va plano. Si dudas dónde guardar algo, va en el módulo del día en el que estás.

## 🧭 Cómo lo uso a diario

1. **Nota del día:** `Ctrl+P` → "Periodic Notes: Open daily note" (se crea en `diario/` con la plantilla).
2. **3 cosas aprendidas + un comando del día** (5 min al cerrar el bloque).
3. **Material durable del día** en el módulo: `diaNN-tema-*.md` (concepto) y `diaNN-lab-*.md` (práctica). **Elige un prefijo de día y dale lleva tu track.**
4. **Domingo:** marca `[x]` en la tabla diaria de arriba y en `M1-fundamentos/tablero.md`.
5. **Sync:** automático cada 30 min con Obsidian abierto (`Ctrl+P` → "Git: Commit-and-sync" para forzar).

Teclas: `Ctrl+O` abrir rápido · `Ctrl+Shift+F` buscar en todo · `Ctrl+E` leer/editar.

## 🕒 Últimas notas

```dataview
TABLE WITHOUT ID file.link AS "Nota", file.mtime AS "Editada"
FROM "diario" OR "M1-fundamentos"
SORT file.mtime DESC
LIMIT 8
```

## 🔒 Notas personales

- Este repo es **público** (muestra evidencia de estudio y progreso — suma al CV).
- ⚠️ Nada de credenciales reales ni datos sensibles: las contraseñas de Bandit van en `M1-fundamentos/diaNN-lab-bandit.md` (cualquier `*bandit*` está en `.gitignore`, no se sube).
- Regla de oro: **un commit por día de estudio** — si no está en el repo, no está hecho.

---
_Actualizado: Día 1 · 2026-09-17 · Semana 1_