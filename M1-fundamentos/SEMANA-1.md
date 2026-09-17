# SEMANA 1 — Arranque: cert + redes base + shell + Git

> Plan día a día (20 h). Leyenda: 🎓 teoría · 🧪 laboratorio · 📝 documentación · 🇬🇧 inglés
> Al terminar la semana, todos los entregables deben estar en el repo `plan-estudios`. Regla del plan: **si no está en el repo, no está hecho.**

## Setup inicial (15 min, una sola vez)

1. Activar **Coursera Plus** → abrir <https://www.coursera.org/professional-certificates/google-cybersecurity> y empezar el **Curso 1 (Foundations of Cybersecurity)**.
2. Descargar e instalar **Git** (si no lo tienes) y **Packet Tracer** (gratis vía <https://www.skillsforall.com> — se necesita cuenta Cisco NetAcad).
3. Crear repo en GitHub: `plan-estudios` (privado), y clonarlo local.

```bash
# Arranque del repo (desde ~/plan-estudios)
git init
git add .
git commit -m "Semana 1 - setup: estructura y plan"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/plan-estudios.git
git push -u origin main
```

Estructura del vault: `diario/` (una nota por día), `M1-fundamentos/` (esta fase: semanas, labs y entregables — todo plano, con prefijo `lab-` / `entregable-`), `plantillas/` (diaria y tema) y `glosario.md` (inglés). Sin subcarpetas: si dudas, va en el módulo actual.

---

## Lunes — Día 1 (3 h): despegar 🎓1.5 + 🧪1.5

- [ ] 🎓 Cert Google Curso 1: módulo 1 — qué es un SOC, por qué existe la ciberseguridad, dominios de seguridad. *(Nota diaria con la plantilla `plantillas/diaria.md`.)*
- [x] 🧪 Shell: `pwd`, `ls`, `cd`, `cat`, `less`, `man` — 30 min en terminal real (TUI/GNOME Terminal).
- [x] 🧪 Git: hacer tu **primer commit del día** con las notas del día. *(Pon en el alias: `git add . && git commit -m "Día 1 ..."`)*

**Hecho cuando:** tienes un commit con las notas del día y sabes explicar qué es un SOC en 2 oraciones.

## Martes — Día 2 (3.5 h): redes base 🎓2 + 🧪1.5

- [ ] 🎓 Modelo TCP/IP vs OSI: capas y para qué sirve cada una (Messer u otro video si hace falta).
- [ ] 🎓 **DNS**: qué resuelve, registros A/AAAA/MX/CNAME, cómo se ve una consulta.
- [ ] 🧪 Comandos `touch`, `mkdir`, `cp`, `mv`, `rm` en el shell (5 min de práctica mental → 20 min de terminal).
- [ ] 🧪 Bandit nivel 0 y 1 (OverTheWire): `ssh bandit0@bandit.labs.overthewire.org -p 2220`, contraseña `bandit0`.

**Hecho cuando:** explicas el flujo de "escribir `google.com` en el navegador → responde el servidor" sin mirar apuntes, y pasaste Bandit 0–1.

## Miércoles — Día 3 (3.5 h): HTTP + shell + Bandit 🎓1.5 + 🧪2

- [ ] 🎓 HTTP/HTTPS y **TLS en 5 ideas**: cifrado, certificados, handshake resumido (ClientHello/ServerHello), por qué HTTPS no es "seguro" por sí solo (certificado correcto ≠ sitio bueno).
- [ ] 🧪 Bandit niveles 2–4 (usar `ls -la`, `cat`, `find` como pista de cada nivel).
- [ ] 🧪 Terminar de practicar `cp/mv/rm` con la estructura de casa (`~/plan-estudios/diario`).

**Hecho cuando:** Bandit 0–4 y puedes explicar el handshake TLS en 3 frases.

## Jueves — Día 4 (3.5 h): Git profesional + Bandit 5 📝1 + 🧪2.5

- [ ] 🧪 Bandit **nivel 5** (el `find` con tamaño de archivo).
- [ ] 🧪 Git: `git status`, `git log --oneline`, `git diff`, deshacer con `git restore`; practicar en el repo.
- [ ] 📝 Estructura de tu carpeta: asegúrate de que `diario/` y `M1-fundamentos/` tengan algo dentro cada una (aunque sea un placeholder honesto).

**Hecho cuando:** Bandit 0–5 ✅ y tienes 3+ commits distintos en el repo.

## Viernes — Día 5 (3 h): teoría de red + README 📝2 + 🎓1

- [ ] 🎓 Ver 1–2 videos de Prof. Messer (Network+) de TCP/IP y DNS para cerrar huecos (YouTube, gratis).
- [ ] 📝 **README.md del repo**: tu contexto (quién eres, qué estudias, objetivo 12 meses) — practicando formato Markdown (títulos, listas, negritas, links).

**Hecho cuando:** el README se lee en 30 segundos y dice tu objetivo.

## Sábado — Día 6 (3.5 h): inglés + cierre 🇬🇧2 + 🧪1.5

- [ ] 🇬🇧 **Glosario SOC** (`glosario.md`): leer los 20 términos, agregar tu propia definición de 1 línea en inglés a cada uno (la del asistente es base; escríbela TÚ con tus palabras).
- [ ] 🇬🇧 Leer en voz alta la intro de <https://attack.mitre.org> (sección "What is ATT&CK?") y anotar 5 palabras nuevas en `glosario.md`.
- [ ] 🧪 Vuelta rápida al shell y Bandit: repetir un nivel que haya costado (refuerzo con memoria muscular).

**Hecho cuando:** glosario con tus definiciones + 5 palabras nuevas anotadas.

## Domingo — Día 7 (libre / flex 0–2 h)

- Descanso real, o amortiguar lo pendiente de la semana (2 h máx). **No empieces la semana 2 atrasado.**

---

## Criterios de "semana 1 completada" (checklist final)

- [ ] Coursera Plus activo y Curso 1 iniciado (primer módulo terminado).
- [ ] Bandit niveles 0–5 completados (screenshot o nota con contraseñas de niveles en `M1-fundamentos/lab-bandit.md`).
- [ ] Repo `plan-estudios` en GitHub con **4+ commits** y README con objetivo.
- [ ] Glosario de 20 términos con tus definiciones en inglés.
- [ ] Notas de cada día usando la plantilla (`plantillas/tema.md`).
- [ ] Commit final del domingo con todo.

## Trampas típicas (evítalas)

1. **El inglés es lo primero que se abandona** — hazlo los sábados antes que cualquier otra cosa.
2. **No "mires" los comandos — típalos.** El shell entra por los dedos, no por los ojos.
3. **No acumules commits de 5 días**: uno por día de estudio mínimo.
4. Si un día no das el objetivo, mueve el bloque entero al domingo-flex, no lo trocees a medias.

---
Siguiente: `MES-1-DETALLADO.md` → Semana 2 (VLAN/NAT + Windows/Event Viewer + Packet Tracer).