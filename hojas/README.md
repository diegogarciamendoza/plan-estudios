# Hojas de recuperación por módulo

> Una hoja por **módulo** de Coursera (`CX-MXX-<slug>.md`). Se abre al empezar el módulo y se cierra el día que apruebas su *module challenge*.
> Plantilla: [`plantillas/hoja-modulo.md`](../plantillas/hoja-modulo.md) · Plan del mes: [`MES-1-DETALLADO.md`](../M1-fundamentos/MES-1-DETALLADO.md)

## Por qué por módulo y no por curso

Decisión tomada el **2026-09-24** con estos datos:

| Motivo | Dato |
|---|---|
| **La unidad de cierre ya es el módulo, no el curso** | El plan cierra cada módulo con su *module challenge* (evidencia: `Module 4 challenge 94.44%`, Curso 1 completo). Una hoja por curso llegaría 4 módulos tarde y habría que reconstruir de memoria lo del primero. |
| **Es lo que se va a releer en el mes 7–8 (Security+)** | 9 cursos × ~4 módulos ≈ **30–36 hojas de 1 página** = el corpus de repaso. Nueve resúmenes de prosa de 6 páginas no se releen; una hoja de preguntas sí. |
| **Lo que a él le falla es producir, no reconocer** | EFSET 2026-09-21: Reading 74 · Listening 81 vs **Writing 59 · Speaking 48**; y **3/8** dominios CISSP producibles de memoria. Un resumen en prosa se **lee** (reconocimiento, ya sobra); una hoja se **responde**. |
| **Coste real por unidad** | 1 página ≈ 10–15 min al cerrar un módulo. El resumen por curso exige re-leer 4 módulos juntos. |

**Regla de llenado:** el *mapa* (nombres de lección) lo deja el asistente; **las respuestas las produce Diego**, en español primero y con los términos en inglés después. El asistente corrige, no escribe las respuestas por él (una hoja llena por otro no recupera nada).

**Qué NO entra aquí:** contenido pegado del curso (transcripts, readings, quizzes) — el repo es público y el material de Coursera vive fuera del vault. Solo *cita* de la lección + palabras propias + fuentes públicas.

## Índice

### Curso 1 — *Foundations of Cybersecurity* ✅ completado 2026-09-22 (`Grade: 90.63%`) · **4 módulos** · **58 términos únicos** de glosario (11 + 19 + 17 + 12 = 59 entradas; `SPII` se repite entre M1 y M3)

| Módulo | Título | Hoja | Estado |
|---|---|---|---|
| M01 | Welcome to the exciting world of cybersecurity | [[C01-M01-welcome-to-cybersecurity]] | 🖊️ retro (repaso) |
| M02 | The evolution of cybersecurity | [[C01-M02-evolution-of-cybersecurity]] | 🖊️ retro (repaso) |
| M03 | Protect against threats, risks and vulnerabilities | [[C01-M03-protect-against-threats]] | 🖊️ retro (repaso) |
| M04 | Cybersecurity tools and programming languages | [[C01-M04-tools-and-programming-languages]] | ✅ llena (ejemplo) |

### Curso 2 — *Play It Safe: Manage Security Risks* · **4 módulos** *(títulos y duraciones verificados 2026-09-24 en la página del curso)*

> ⏰ **Vence:** `Module 1 challenge` Sep 28 · `Module 2 challenge` + *Portfolio Activity: Conduct a security audit* **Oct 2** (5% del curso) · `M3 challenge` Oct 7 · `M4 challenge` Oct 9.

| Módulo | Título | Duración | Hoja | Estado |
|---|---|---|---|---|
| M01 | Security domains | 2h18m | [[C02-M01-security-domains]] | ✅ **100%** (2026-09-24) |
| M02 | Security frameworks and controls *(aquí entra OWASP)* | 3h07m | | ⬜ |
| M03 | Introduction to cybersecurity tools *(SIEM, dashboards)* | 1h40m | | ⬜ |
| M04 | Use playbooks to respond to incidents | 1h55m | | ⬜ |

### Cursos 3–9 *(títulos verificados 2026-09-24; nº de módulos por verificar cuando toque)*

| # | Curso | Hoja |
|---|---|---|
| 3 | Connect and Protect: Networks and Network Security | ⬜ |
| 4 | Tools of the Trade: Linux and SQL | ⬜ |
| 5 | Assets, Threats, and Vulnerabilities | ⬜ |
| 6 | Sound the Alarm: Detection and Response | ⬜ |
| 7 | Automate Cybersecurity Tasks with Python | ⬜ |
| 8 | Put It to Work: Prepare for Cybersecurity Jobs | ⬜ |
| 9 | Accelerate Your Job Search with AI | ⬜ |

## Fuentes del plan (verificadas)

### Las que trajo Diego (2026-09-24)

| Fuente | Veredicto | Dónde encaja |
|---|---|---|
| <https://owasp.org/projects/top-ten> | ✅ **vigente** — la versión actual es **OWASP Top 10:2025** (`A01 Broken Access Control` … `A10 Mishandling of Exceptional Conditions`; verificado en `top10.owasp.org/2025`) | **Curso 2 · M02**, donde aparece la lección *OWASP security principles*. ⚠️ Ojo: **no es la misma lista** — la lección cubre los *principios*, esta URL son los **10 riesgos**. La que más te va a tocar en un SOC es **A09 Security Logging and Alerting Failures**. |
| <https://www.cisa.gov/resources-tools/resources/no-cost-cybersecurity-services-and-tools> | ✅ **vigente** (HTTP 200, 2026-09-24). Contiene: *Cyber Hygiene Services* (escaneo de sistemas expuestos), *CPG Assessment*, catálogo **KEV** y una base de herramientas gratis filtrable por nivel (Foundational / Intermediate / Advanced) y por los 38 CPG IDs | **Curso 8** (empleo) y como lista de herramientas gratis para el lab del mes 3. ⚠️ Los *servicios* son para organizaciones de **EE.UU.**; la base de **herramientas** aplica a cualquiera. |
| Threat Horizons **sept-2022** (PDF) | ⚠️ **desactualizado**: son datos de Q2-2022 y ya hay ediciones mucho más nuevas (**H2 2025** = 12.ª edición, y **H1 2026**). Sirve como **ejemplo del formato** de un informe de threat intel, no como dato vigente. | **Curso 5/6** (amenazas / detección). Si se cita una cifra, citar la edición vigente: <https://cloud.google.com/security/report>. El hallazgo literal de ese número: en Q2-2022 *"weak and default-password issues … factoring in over half of identified incidents"* → entonces **más de la mitad** de los incidentes empezaron por credenciales débiles o por defecto (SSH, WordPress, RDP) y **65%** terminaron en criptominería. |
| Docs de Google `1QrlsTDX…` (`/template/preview`) | 🚫 **descartado** (2026-09-24): HTTP **404** sin sesión y Diego no lo tiene a mano — si reaparece, se integra | — |
| Docs de Google `1bBtBHYr…` → **identificado: Glosario del Curso 1** (plantilla de Google Docs del propio certificado; la lección *07_Course 1 glossary* del export de momo **es el enlace a este Doc**) | ⚠️ **material del curso → no entra al vault**. Contado y cotejado 2026-09-24: **58 términos**, **56 en común** con los glosarios de módulo (11+19+17+12 = 59 entradas, `SPII` repetida). Aporta `Open Web Application Security Project (OWASP)` y `Adversarial artificial intelligence` (sin `(AI)`); **no** trae `CISSP` (que sí está en el glosario del módulo 2) | Uso: **checklist contable del Curso 1** (58 términos) para el repaso final del curso y para Security+. La fuente autoritativa **por módulo** son las lecciones *Glossary terms from module N* |

### Transversales (ya en el plan)

| Fuente | Para qué |
|---|---|
| <https://attack.mitre.org> | Tácticas/técnicas (desde el Curso 6) |
| <https://learn.microsoft.com> | Event IDs de Windows (4624/4625/4672/4688) |
| <https://www.elastic.co/docs> | Documentación de SIEM |
| <https://professormesser.com> | Repaso en video Network+/Security+ |

---
_Actualizado: 2026-09-24_
