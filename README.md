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

| Fase | Periodo | Contenido | Certificación |
|---|---|---|---|
| M0 | Mes 0 | Fundamentos fisgones (Linux, redes base), test de vocación | — |
| M1 | Meses 1–2 | Google Cybersecurity Certificate + TryHackMe SOC | Google (Coursera) |
| M2 | Meses 7–8 | Security+ SY0-701 | **Security+** 🎯 |
| M3 | Meses 9–12 | Especialización por vacantes + CySA+ solo si aplica | CySA+/eJPT (opcional) |

📄 [GENERAL.md](GENERAL.md) — plan completo · 📅 [MES-1-DETALLADO.md](M1-fundamentos/MES-1-DETALLADO.md) — mes 1
🧭 [SEMANA-1.md](M1-fundamentos/SEMANA-1.md) — semana actual · 📋 [Tablero](M1-fundamentos/tablero.md)

## 📈 Progreso semanal

| Semana | Tema | Estado | Entregables |
|---|---|---|---|
| 1 | Cert + redes base + shell + Git | 🔄 en curso | Bandit 0–5, repo+commits, glosario 20 |
| 2 | VLAN/NAT + Windows/Event Viewer | ⬜ pendiente | Packet Tracer, 5 cmds PowerShell, 4625 |
| 3 | Linux a fondo + SQL + Python | ⬜ pendiente | 10 consultas SQL, script fuerza bruta |
| 4 | Wireshark + MITRE + SIEM + CV | ⬜ pendiente | Investigación 1 pág, mapa de red, CV |

_Leyenda: ✅ hecho · 🔄 en curso · ⬜ pendiente_

## 📁 Estructura

```
plan-estudios/
├── README.md           ← este archivo (índice, progreso y últimas notas)
├── GENERAL.md          ← plan de 12 meses (el mapa)
├── glosario.md         ← inglés: términos SOC (crece todo el año)
├── vacantes-*.md       ← mercado laboral (referencia)
├── diario/             ← una nota por día de estudio (YYYY-MM-DD)
├── M1-fundamentos/     ← fase actual: MES-1-DETALLADO, SEMANA-N, lab-*, entregable-*
├── M2-security-plus/   ← meses 7-8
├── M3-especializacion/ ← meses 9-12
└── plantillas/         ← diaria.md (nota del día) · tema.md (nota de estudio)
```

**Regla:** dentro de un módulo todo va plano (sin subcarpetas). Si dudas dónde guardar algo, va en el módulo en el que estás ahora.

## 🧭 Cómo lo uso a diario

1. **Nota del día:** `Ctrl+P` → "Periodic Notes: Open daily note" (se crea sola en `diario/` con la plantilla).
2. **3 bullets de lo aprendido + un comando del día.** 5 minutos al cerrar el bloque de estudio.
3. **Labs y entregables:** en el módulo actual, con prefijo `lab-` o `entregable-`.
4. **Domingo:** ✅ en la tabla de progreso de arriba y en `M1-fundamentos/tablero.md`.
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
- ⚠️ Nada de credenciales reales ni datos sensibles: **las contraseñas de Bandit van en `M1-fundamentos/lab-bandit.md` (y cualquier archivo `lab-bandit*.md` está en `.gitignore`, no se suben)**.
- Regla de oro: **un commit por día de estudio** — si no está en el repo, no está hecho.

---
_Actualizado: 2026-09-16 · Semana 1_