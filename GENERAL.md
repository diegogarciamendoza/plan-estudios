# Plan de Estudios — Ciberseguridad / SOC (Diego) · Resumen General

> Fuente autoritativa: `~/wiki/concepts/plan-carrera-ciberseguridad.md` (v3, revisado por Luna, 2026-09-16)
> Detalle del primer mes: [`MES-1-DETALLADO.md`](./MES-1-DETALLADO.md)

## Perfil

- Edad 40+, México. Disponibilidad: **20+ h/semana**.
- Inglés: **técnico intermedio** (módulo aplicado a SOC, no curso general). **Medido 2026-09-21** con [EFSET 4-skills](https://cert.efset.org/en/uMnF3B): **C1 global (66/100)** — Reading 74 · Listening 81 · Writing 59 (B2) · Speaking 48 (B1) → el cuello de botella es la **producción**, no la comprensión.
- Presupuesto mensual: **$300–1,000 MXN** + **Coursera Plus YA activo (patrocinado por un familiar)**.
- Base actual: programación intermedia · Linux básico · reparación de PCs · redes básicas · electrónica incompleta · power user.

## Modo actual (desde 2026-09-21)

> **Dos frentes: Coursera + inglés.** Todo lo demás queda **pausado con condición de reactivación**, no abandonado — detalle en [[MODO-CURSERA-INGLES]].
> Motivo: el certificado Google Cybersecurity **ya cubre Linux, SQL, Python, redes y detección**; practicarlo en paralelo duplicaba esfuerzo y dispersaba el foco (riesgo nº 1 del plan).
> Inglés: sube de 15 a **25 min/día** + la sesión del sábado, ahora con **pronunciación** (5 min diarios). Prioridad si el día no alcanza: **Coursera ≥ inglés ≥ lo demás**.

## Objetivo (12 meses)

> **"Demostrar competencias de SOC L1 con tres investigaciones reproducibles, un laboratorio funcional, Security+ si el presupuesto lo permite y experiencia real de postulación/entrevista."**

El objetivo a 12 meses es **ser empleable y conseguir entrevistas**, no tener el trabajo ideal. El primer empleo puede ser soporte o NOC — es parte del plan.

## El plan en 6 fases

| Fase | Meses | Foco | Cierre / entregable |
|---|---|---|---|
| 1 | 1–2 | **Fundamentos SOC** (Google Cybersecurity Certificate + base técnica) | Mapa de red, consultas SQL, PowerShell, Wireshark, CV técnico |
| 2 | 3–4 | **Operaciones de seguridad** (logs, Sysmon, SIEM, phishing, triage) | Proyecto fuerza bruta + phishing, primer repo público, **primeras postulaciones (semana 8–12, no esperar Security+)** |
| 3 | 5–6 | **Laboratorio defendible** (1 VM Windows + 1 VM Ubuntu + Wazuh **o** Elastic + Sysmon) | Lab reproducible, 3 casos de investigación, portfolio para entrevistas |
| 4 | 7–8 | **Security+ SY0-701** — única cert paga del año | Examen aprobado (si aplica, ver regla abajo) |
| 5 | 9–10 | **Especialización según vacantes** (elegir UNA: Microsoft/Defender · redes/firewalls · SIEM/detección · cloud básico) | Decisión basada en qué repiten las vacantes reales |
| 6 | 11–12 | **Empleo + decisión de 2ª cert** | CySA+/CCNA/eJPT SOLO si una vacante la pide, el portafolio está listo, no rompe presupuesto y hay razón laboral concreta |

Puertas de entrada realistas: help desk con tareas de seguridad → NOC junior → monitoreo → vulnerability management junior → SOC L1 trainee → MSP → Soporte/NOC → SOC L1.

## Reglas de oro

1. **UNA sola certificación paga: Security+ (~$425–439 USD ≈ $7,300–7,500 MXN).** Comprar el examen **SOLO si**: simulacros >80–85%, puedes explicar el porqué de cada respuesta, y hay dinero separado para un 2º intento. Español disponible (verificar fechas con CompTIA; SY0-701 retira español en 2027-08). Renovación: 50 CEUs / 3 años.
2. **Certificaciones gratuitas (Cisco NetAcad, etc.) sí**: aportan al CV y dan motivación real.
3. **Portafolio > certificaciones**: 3 investigaciones reproducibles (ver abajo).
4. **Sin malware real en el lab**: solo eventos de autenticación, PowerShell, procesos, DNS y simulaciones controladas (Atomic Red Team).
5. **Ventana de postulación a las 8–12 semanas**, no al final del año.

## Distribución semanal (20 h)

| Bloque | Horas |
|---|---|
| Teoría | 8 |
| Laboratorio | 8 |
| Documentación / portafolio | 2 |
| Empleo / CV / **inglés aplicado a SOC** | 2 |

## Portafolio: 3 proyectos (valen más que otra cert)

1. **Investigación de fuerza bruta** — captura/dataset, consulta de fallos de auth, umbral justificado, falsos positivos, timeline, informe de 1 página.
2. **Detección de PowerShell sospechoso** — Event IDs, Sysmon/logs Windows, consulta SIEM, caso benigno vs. sospechoso, mapeo MITRE.
3. **Phishing** — headers, dominio/URL, SPF/DKIM/DMARC, IOC, respuesta recomendada, ticket simulado.

Cada repo: README, arquitectura, pasos de reproducción, consultas, screenshots, resultados, falsos positivos, "qué haría después" y aviso de laboratorio.

## Presupuesto anual (~$7,500–9,000 MXN total)

- Meses 1–6: **$0–300/mes** (todo gratis o casi gratis; Coursera Plus ya pagado por el familiar).
- Meses 7–8: ahorrar para Security+.
- Meses 9–12: examen único comprado cuando esté preparado.
- **No pagar**: TryHackMe Premium (máximo 1–2 meses puntuales), libros nuevos (biblioteca/2ª mano/gratis).
- Si el voucher excede el presupuesto: esperar y ahorrar, promo oficial/voucher regional, o portafolio + aplicar sin cert.

## Riesgos (previstos, no sorpresas)

- **Turnos/condiciones**: muchos SOC L1 son 24/7 — noche, rotación, presencial, monotonía. Evaluar turnos, transporte y guardias desde el inicio (no idealizar el primer empleo).
- **Edad (40+)**: no ocultarla ni hacerla el centro. El CV se plantea como transición técnica con experiencia previa: resolución de problemas, reparación, autonomía, disciplina.
- **Inglés**: es el módulo que más se abandona. 2 h/semana fijas, aplicadas a SOC (resumen ejecutivo, documentación oficial, entrevistas), no un curso general. **Arreglo 2026-09-20:** esas 2 h se reparten en **15 min diarios + la sesión larga del sábado**, y el foco pasa de *leer* a **producir** (diagnóstico medido: 3/8 dominios CISSP producibles de memoria, aunque sí se reconocen al leerlos). La práctica oral va enganchada al repaso SRS (el reverso en inglés **se dice en voz alta** antes de graduar) para que no cueste minutos extra. Métrica de cierre por módulo: producir de memoria en inglés los términos técnicos del módulo (dominios CISSP, tipos de ataque) antes de darlo por cerrado. Subtítulos del curso **en inglés, nunca en español**.
- **Inglés — medición externa y arreglo 2026-09-21 (EFSET 4-skills)**: [certificado](https://cert.efset.org/en/uMnF3B) → **C1, 66/100** · Reading **74** (C2) · Listening **81** (C2) · **Writing 59 (B2)** · **Speaking 48 (B1)**. Lectura: no es falta de inglés, es **producción en tiempo real** (oír 81 ↔ hablar 48 = 33 puntos; escribir rinde más que hablar porque da tiempo a recuperar y corregir). Consecuencias: (1) los 15 min diarios pasan a **≥70% producción** en rotación escritura/oral; (2) el sábado produce **1 artefacto escrito en inglés** = a la vez entregable del portafolio (informe de incidente, executive summary, ticket de phishing); (3) leer y escuchar **no tienen tiempo asignado** (ya C2, siguen como insumo del curso); (4) feedback del asistente con rúbrica + **bitácora de errores** → tarjetas SRS solo de errores recurrentes; (5) retest EFSET 4-skills a los ~3 meses (gratis, <https://www.efset.org/4-skill/>).

## Salarios (usar con cautela)

Los datos de Indeed/Glassdoor tienen muestras diminutas y mezclan mensual/anual. Antes de decidir especialidad o negociar: revisar **20–30 vacantes reales** de México, registrar salario/ciudad/modalidad/turnos/requisitos y calcular la mediana.

## Pendientes / siguientes pasos

- [ ] Análisis de 20–30 vacantes reales (México) — agente en background.
- [ ] Ejecutar el Mes 1 (ver `MES-1-DETALLADO.md`).