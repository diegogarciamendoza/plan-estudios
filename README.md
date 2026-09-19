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

📄 [GENERAL.md](GENERAL.md) — el plan completo (12 meses) · 📅 [MES-1-DETALLADO.md](M1-fundamentos/MES-1-DETALLADO.md) · 🧭 [SEMANA-1.md](M1-fundamentos/SEMANA-1.md)

## 📌 Día actual

**▶️ Día 3** · [diario/2026-09-19.md](diario/2026-09-19.md)

## 📈 Progreso diario (en qué día voy)

_`[x]` hecho · `[ ]` pendiente — marca al cerrar cada día de estudio; el link va a la nota del día._

| Día | Tema | Estado |
|---|---|---|
| **01** | Shell: `pwd ls cd cat less man` | ✅ [nota](diario/2026-09-17.md) |
| 02 | Redes TCP/IP + DNS + Linux self-paced (TryHackMe) | 🔄 [nota](diario/2026-09-18.md) · falta DNS |
| 03 | HTTP/TLS + Bandit 2–4 | 🔄 [nota](diario/2026-09-19.md) |
| 04 | Git + Bandit 5 | ⬜ |
| 05 | Messer Network + README | ⬜ |
| 06 | Inglés + glosario SOC | ⬜ |

_Leyenda: ✅ hecho · 🔄 en curso · ⬜ pendiente_

## 📁 Estructura

```
plan-estudios/
├── README.md            ← este archivo (panel: mapa, progreso, día actual)
├── GENERAL.md           ← plan de 12 meses (referencia, se lee al planear)
├── glosario.md          ← inglés: términos SOC (crece todo el año)
├── vacantes-*.md        ← mercado laboral (referencia)
├── diario/              ← 1 nota por día, TODO el día: YYYY-MM-DD.md
├── M1-fundamentos/      ← solo lo durable: SEMANA-N, MES-1, tablero, entregables grandes
├── M2-security-plus/    ← meses 7-8
├── M3-especializacion/  ← meses 9-12
└── plantillas/          ← diaria.md (única plantilla por defecto)
```

**Regla (KISS):** lo de cada día va en `diario/YYYY-MM-DD.md`, con todo junto (aprendí + práctica + duda). Solo sube al módulo lo que de verdad va a **crecer o reutilizarse** (glosario, scripts, entregables grandes). Si dudas, va al diario — nada de decidir tipos por cada nota.

## 🧭 Cómo lo uso a diario

1. **Nota del día:** `Ctrl+P` → "Periodic Notes: Open daily note" (se crea en `diario/` con la plantilla).
2. **Todo el día ahí**: aprendí + comandos + práctica + duda. 5 min al cerrar el bloque.
3. **Tablero semanal** ([tablero.md](M1-fundamentos/tablero.md)): muevo lo hecho a "Hecho" el domingo (o yo lo actualizo).
4. **README**: marco `[x]` en la tabla diaria y enlazo la nota del día.
5. **Sync:** automático cada 30 min con Obsidian abierto (`Ctrl+P` → "Obsidian Git: Commit-and-sync" para forzar; si falla, ver "cómo resolver pull" abajo).

Teclas: `Ctrl+O` abrir rápido · `Ctrl+Shift+F` buscar en todo · `Ctrl+E` leer/editar.

## 🔒 Notas personales

- Este repo es **público** (muestra evidencia de estudio y progreso — suma al CV).
- ⚠️ Nada de credenciales reales ni datos sensibles: cualquier `*bandit*.md` está en `.gitignore`, no se sube.
- Regla de oro: **un commit por día de estudio** — si no está en el repo, no está hecho.

## 🔧 Trouble-shooting del sync (Windows)

- **Pull failed (merge)**: hay cambios locales sin commitear que el pull no puede sobrescribir → `git stash` → `git pull` → `git stash pop`. Si `pop` da `deleted by us`, es un archivo viejo eliminado: descartarlo con `git rm` y `git stash drop`.
- **"Modified" fantasma** (LF↔CRLF, diff vacío): costumbre de Obsidian en Windows; descartar con `git checkout -- <archivo>`.

---
_Actualizado: Día 3 · 2026-09-19 · Semana 1_