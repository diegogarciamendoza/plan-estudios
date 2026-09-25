---
tipo: hoja-modulo
curso: 1
modulo: 4
estado: cerrada
abierta: 2026-09-22
cerrada: 2026-09-22
tags:
  - hoja-modulo
  - coursera
enlaces:
  - hojas/README
  - diario/2026-09-22
  - M1-fundamentos/tablero
---

# C1 · M04 — Cybersecurity tools and programming languages

> **Curso 1 *Foundations of Cybersecurity* · módulo 4 de 4.** Cerrado el **2026-09-22** con *Module 4 challenge* **`94.44%`** (curso completo: `90.63%`, [[2026-09-22]]).
> **Esta hoja es el EJEMPLO del formato** — está llena con material **tuyo** (tu nota del día, tus definiciones, el análisis de tu toma oral), para que la de los demás módulos se vea igual. Las respuestas están en callouts plegados: se destapan **después** de decirlas.

**Hecho cuando:** ✅ *module challenge* 94.44% · ✅ mapa completo · ✅ 3 términos producidos de memoria (voz + escrito) · ✅ fuentes marcadas.

## En una frase

> Un analista de SOC vive dentro de **herramientas** (SIEM, sniffer) y necesita **leer y consultar datos** (logs) para decidir qué escalar — el módulo pone nombre a esas piezas y a los lenguajes que las manejan (Linux, SQL, Python). *(borrador del asistente desde tu oral del 22 — corrígelo con tus palabras)*

## Mapa del módulo

| # | Lección (nombre real) | Qué me llevo (1 línea, mía) |
|---|---|---|
| 1 | Tools for protecting business operations | Qué herramientas entran en un SOC y para qué protege cada una *(borrador)* |
| 2 | Common cybersecurity tools | SIEM y analizador de protocolos/packet sniffer son las dos del rol de nivel inicial *(borrador)* |
| 3 | Use tools to protect business operations | El SIEM **centraliza logs**; el sniffer **mira el tráfico** *(borrador)* |
| 4 | Introduction to Linux, SQL, and Python | Linux = el sistema donde viven los logs · SQL = consultarlos · Python = automatizar *(borrador)* |

## Recuperación (decir de memoria, después destapar)

**1. ¿Qué es un log?**
> [!success]- Mi respuesta (tuya, 2026-09-22)
> *"A log is a record of events that occur within an organization's systems"* — corregido en sesión: `within` + plural `systems` (habías puesto `in an organization's syst…`).

**2. ¿Qué es un SIEM y de dónde saca la información?**
> [!success]- Mi respuesta (tuya, 2026-09-22)
> *"SIEM — Security Information and Event Management — is an application that collects and analyzes log data to monitor critical activities in an organization."* Corregido: `collects and analyzes` (los dos verbos en 3.ª persona) y `in **an** organization` (definición genérica → artículo indefinido).

**3. ¿Cuál es la diferencia entre un SIEM y un analizador de protocolos de red? ¿Cuándo usarías cada uno?**
> [!success]- Mi respuesta
> — *(pendiente: respóndelo tú. Pista de forma: uno **centraliza** lo que ya está registrado; el otro **captura** lo que está pasando ahora en el cable.)*

**4. Corrige tu propia frase del oral: *"the safeguards that reduce a specific risk, or security controls, are SIEM"*. ¿Qué tiene de impreciso?**
> [!success]- Corrección (2026-09-22)
> El SIEM es **una** de esas salvaguardas, no todas: *"SIEM is **one of** the security controls."* El error es **cuantificador** (de *todos* a *uno*), no de vocabulario.

**5. ¿Por qué un analista de SOC necesita Linux y SQL todos los días?**
> [!success]- Mi respuesta
> — *(pendiente: respóndelo tú; conéctalo con los logs que ya tocaste en `/var/log` y con lo que hiciste el Día 3.)*

## Inglés — producción del módulo

Términos del glosario del módulo 4 (tiene **12**; estos 3 son los que se producen de memoria, dichos y escritos).

| # | Término (EN) | Lo dije en voz alta | Lo escribí | Una frase mía usándolo |
|---|---|---|---|---|
| 1 | log | ⚠️ el STT oyó **"lock"** (la `-g` final se ensordece) | ✅ `log` | *"A log is a record of events within an organization's systems."* |
| 2 | network protocol analyzer (packet sniffer) | ⚠️ el STT oyó **"sneaker"** (la `/f/` no cierra) | ✅ `network protocol analyzer` (ortografía corregida: `analyzer`) | *"A packet sniffer captures and analyzes network traffic."* |
| 3 | SIEM | ✅ `/sɪm/` (el propio curso lo dice así: *sim* o *seem*) | ✅ `SIEM` | *"A SIEM collects and analyzes log data to monitor critical activities."* |

> Medición real de la toma de 99,5 s (2026-09-22): **77 pal/min** · 2 pausas ≥1 s · 48,1 s de habla continua. El cruce **escritura ↔ STT** aisló la causa: **escribes bien `log` y `packet sniffer`** → lo que falla es **pronunciación**, no vocabulario.

## Fuentes

| Fuente | Qué cubre de este módulo | Verificada |
|---|---|---|
| — (sin fuente externa propia para este módulo) | Las tres que trajo Diego encajan en **C2-M02** (OWASP), **C5/C6** (Threat Horizons) y **C8** (CISA) — ver [[hojas/README]] | 2026-09-24 |

## SRS

| Tarjeta (frente → reverso) | Por qué existe |
|---|---|
| definición EN → término: *"A record of events that occur within an organization's systems"* → `log` | error propio (ortografía y pronunciación) |
| definición EN → término: *"collects and analyzes log data to monitor critical activities"* → `SIEM` | error propio (artículo + concordancia) |
| definición EN → término: *"a tool designed to capture and analyze network traffic"* → `packet sniffer` | error propio (participio `designed`) |

## Bloqueos y dudas abiertas

| Duda | Qué probé / qué leí | Sigue abierta |
|---|---|---|
| ¿El SIEM también *responde*, o solo *informa*? | Lección *Playbooks, SIEM tools, and SOAR tools* (Curso 2, M04) | Sí — se resuelve en el Curso 2 |

---
_Actualizada: 2026-09-24_
