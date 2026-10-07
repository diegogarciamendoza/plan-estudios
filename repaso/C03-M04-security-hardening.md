---
tipo: hoja-modulo
curso: C03
modulo: M04
estado: abierta
abierta: 2026-10-07
cerrada:
tags:
  - hoja-modulo
  - curso-3
enlaces:
  - repaso/README
  - M1-fundamentos/MES-1-DETALLADO
  - cursos/google-cybersecurity/curso-03-connect-and-protect
---

# C03 · M04 — Security hardening

> **Curso 3 *Connect and Protect: Networks and Network Security* · módulo 04 de 04 — cierra el curso.** Duración: la muestra la plataforma.
> Se abre el día que **empieza** el módulo (2026-10-07) y se cierra el día que apruebas su *module challenge*.
> Una hoja = un módulo. Nunca un resumen por curso (el motivo está en [[repaso/README]]).

**Cómo se usa (3 reglas):**

1. **Se responde, no se lee.** La respuesta vive dentro de un callout plegado `> [!success]-`: primero la dices/escribes de memoria, **después** la destapas.
2. **Aquí no entra contenido del curso.** El *mapa* cita la lección (para saber de dónde sale); lo demás son **tus palabras** en español + tus términos en inglés. Nada de pegar transcripts: el repo es público y el material de Coursera vive fuera ([[MES-1-DETALLADO]] → *cómo obtenerlo*).
3. **Se llena mientras estudias**, no al final de golpe: la lección que cierras hoy deja su fila y su pregunta hoy.

**Hecho cuando:** *module challenge* **≥80%** + mapa completo (todas las lecciones) + **los 10 términos del módulo producidos en inglés** (dichos en voz alta *y* escritos) + fuentes marcadas.

## En una frase

> ¿Qué problema del trabajo real resuelve este módulo? (una frase tuya, sin copiar)

## Mapa del módulo

*Nombres reales de las lecciones, leídos del export del curso el 2026-10-07 (orden del export; el de la plataforma puede variar).*

| # | Lección (nombre real) | Qué me llevo (1 línea, mía) |
|---|---|---|
| 1 | Welcome to module 4 | |
| 2 | Brute force attacks and OS hardening | |
| 3 | Security hardening | |
| 4 | Activity: *Apply OS hardening techniques* (con ejemplar) | |
| 5 | OS hardening practices | |
| 6 | Network security applications | |
| 7 | Network hardening practices | |
| 8 | Activity: *Analysis of network hardening* (con ejemplar) | |
| 9 | Network security in the cloud | |
| 10 | Secure the cloud | |
| 11 | Cryptography and cloud security | |
| 12 | Glossary terms from module 4 | |
| 13 | Wrap-up | |
| 14 | **Course wrap-up** *(cierra el Curso 3)* | |
| 15 | Reflect and connect with peers | |
| 16 | Course 3 glossary | |
| 17 | Get started on the next course *(Curso 4 — Tools of the Trade: Linux and SQL)* | |
| — | *Vídeo de rol*: Kelsey — Cloud security explained | |

> ⚠️ El export trae el **ejemplar** de las dos actividades, no el enunciado calificado: al llegar a ellas, apunta en la nota del día si son **calificadas** (`Submitted · Graded`) y su porcentaje. Los informes que producen (*Security incident report* / *Security risk assessment*) son **entregables del portafolio**: se reformatean al formato propio (alcance · supuestos · método · hallazgos · límites), no se pega la plantilla de Google.

## Recuperación (decir de memoria, después destapar)

**1. Define *security hardening* con tus palabras y da **una medida concreta por superficie**: sistema operativo, red, aplicación y nube.**
> [!success]- Mi respuesta
> _(dila en voz alta y escríbela aquí; si te trabas, anótalo — el bloqueo es el dato)_

**2. *Baseline configuration*: ¿por qué sin baseline no hay hardening, y qué se hace cuando un sistema se desvía de ella?**
> [!success]- Mi respuesta
> _(la pregunta de *cuál y por qué* es la que más te saltas: respóndela escrita, no mental)_

**3. Separa estas tres cosas por lo que cada una ataca: *patch update*, *baseline image* y *backup*.**
> [!success]- Mi respuesta
> _(transferencia: vulnerabilidad / configuración / pérdida de datos — di cuál es cuál y por qué)_

**4. *World-writable file* y *brute force*: ¿por qué el primero es un riesgo de escalada y cómo lo buscarías en un sistema Linux? ¿Qué complementa a la contraseña contra el segundo y qué NO es MFA?**
> [!success]- Mi respuesta
> _(dos ideas que en el trabajo se piden juntas: reconocer el archivo flojo y cerrar la puerta de acceso)_

## Inglés — producción del módulo

Los términos son los **10 del glosario del módulo** (lección *Glossary terms from module 4*); se cierran **diciéndolos de memoria en voz alta y escribiéndolos**: si el término se produce mal (forma, acrónimo, artículo), va a tarjeta SRS.

| # | Término (EN) | Lo dije en voz alta | Lo escribí | Una frase mía usándolo |
|---|---|---|---|---|
| 1 | Baseline configuration (baseline image) | | | |
| 2 | Hardware | | | |
| 3 | Multi-factor authentication (MFA) | | | |
| 4 | Network log analysis | | | |
| 5 | Operating system (OS) | | | |
| 6 | Patch update | | | |
| 7 | Penetration testing (pen test) | | | |
| 8 | Security hardening | | | |
| 9 | Security information and event management (SIEM) | | | |
| 10 | World-writable file | | | |

## Fuentes

Solo fuentes **públicas y verificadas** (fecha de verificación incluida). El mapa de todas las del plan vive en [[repaso/README]].

| Fuente | Qué cubre de este módulo | Verificada |
|---|---|---|
| <https://www.cisecurity.org/cis-benchmarks> | **Baselines de configuración por producto**: la versión real y pública de lo que el módulo llama *baseline configuration* | ✅ HTTP 200 · 2026-10-07 |
| <https://www.cisa.gov/known-exploited-vulnerabilities-catalog> | **Patching con criterio**: la lista de vulnerabilidades explotadas de verdad (prioriza sobre el CVSS a secas) | ✅ HTTP 200 · 2026-10-07 |
| <https://csrc.nist.gov/pubs/sp/800/40/r4/final> | NIST SP 800-40r4 — guía de **gestión de parches** (*patch update*) | ✅ HTTP 200 · 2026-10-07 |
| <https://pages.nist.gov/800-63-4/sp800-63b.html> | NIST SP 800-63B **rev. 4** — autenticadores y **MFA**; sustituye a la 63-3 | ✅ HTTP 200 · 2026-10-07 |
| <https://attack.mitre.org/techniques/T1110/> | **Brute Force** (ATT&CK) — el ataque de la primera lección | ✅ HTTP 200 · 2026-10-07 |
| <https://man7.org/linux/man-pages/man1/chmod.1.html> | Permisos en Linux: qué significa *world-writable* en bits, no en prosa | ✅ HTTP 200 · 2026-10-07 |
| <https://www.rfc-editor.org/rfc/rfc4251.html> | SSH — el canal que se endurece (puerto, root, claves) | ✅ HTTP 200 · 2026-10-07 |

## SRS

| Tarjeta (frente → reverso) | Por qué existe |
|---|---|
| | error propio · concepto umbral |

## Bloqueos y dudas abiertas

| Duda | Qué probé / qué leí | Sigue abierta |
|---|---|---|
| | | |

---
_Actualizada: 2026-10-07_
