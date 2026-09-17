# Mercado laboral TI junior → ciberseguridad defensiva (SOC) en México
**Informe de mercado laboral — vacantes reales (septiembre 2026)**
Fecha de recopilación: 16 de septiembre de 2026. Preparado para perfil junior en transición de soporte TI/NOC a SOC.

---

## 1) Metodología

- **Qué se buscó**: vacantes activas para roles de entrada al mundo SOC: soporte técnico TI, mesa de ayuda, NOC junior, analista SOC N1, analista de ciberseguridad junior, con énfasis en salario publicado, requisitos, modalidad y turnos.
- **Fuentes**: bolsas de trabajo mexicanas (Computrabajo MX, OCC, SNE-Empleo.gob.mx, bebee/Indeed) y páginas salariales agregadas (Indeed Career, Glassdoor, Jooble) solo como contexto estimado.
- **Búsquedas realizadas** (16/09/2026): `analista SOC nivel 1 vacante México`, `NOC junior vacante México sueldo`, `soporte técnico TI vacante México sueldo`, `analista ciberseguridad junior remoto México SIEM`, `"analista SOC" "Security+" junior turnos 24/7`, `SOC L1 Guadalajara/Monterrey/Querétaro salario`, más páginas de listados de Computrabajo (`trabajo-de-soc`, `trabajo-de-monitoreo-noc`, `trabajo-de-analista-de-ciberseguridad`, `trabajo-de-soporte-tecnico`) y OCC (`empleos/de-soc/en-mexico/`).
- **Vacantes recopiladas**: **28 vacantes concretas** — **27 con monto de salario publicado** (26 reportados por el empleador en Computrabajo + 1 "neto" en listado bebee/Indeed) y **1 sin monto publicado** (SNE: "sueldo 100% nominal"). De ellas, 26 provienen de Computrabajo (se extrajo el texto completo de cada oferta: salario, empresa, ciudad, requisitos, turnos); 2 provienen de bebee (listados originados en Indeed) y SNE (empleo.gob.mx).
- **Reglas de rigor aplicadas**:
  - Solo se cuentan salarios **publicados explícitamente por la vacante** (list price del empleador). Cuando no aparece, se escribe **no reportado**.
  - Todos los salarios de Computrabajo incluyen la unidad `(Mensual)` dentro de la oferta → sin ambigüedad anual/mensual salvo que se indique.
  - Se marcó con `[ESTIMADO]` todo dato agregado (calcular promedios) que NO proviene de una vacante individual.
  - "Ingeniero SOC Jr" (AIT, Hermosillo) y "Mesa de control operativa" (CDMX): experiencias detectadas por regex (15 años) son falsos positivos de parseo; el dato relevante citado es el publicado por la empresa.

---

## 2) Tabla resumen de salarios por rol (MXN/mes)

**Fuente de esta sección**: salarios **reportados por las propias vacantes** (list price del empleador) en Computrabajo, septiembre 2026. n = número de vacantes distintas con sueldo publicado en ese rol.

| Rol | n | Mediana (MXN/mes) | Rango reportado (min–max) | Notas |
|---|---|---|---|---|
| **SOC L1 / monitoreo SOC junior** | 5 | **$18,000** | $10,000 – $25,000 | La vacante de $10,000 es explícitamente para recién egresados (Grupo Pryse). Varias piden 6 meses–2 años de experiencia. |
| **Analista de seguridad junior** (ciberseguridad/seguridad de la información) | 9 | **$23,000** | $17,000 – $35,000 | Mayoría pide 1–3 años de experiencia; no son roles de primer empleo. Incluye analista SOC con 2 años (Naucalpan $27,000). |
| **NOC / monitoreo de red junior** | 6 | **$14,000** | $12,000 – $18,604 | Turnos rotativos comunes (12 h, rolados 24/7). |
| **Soporte TI / mesa de ayuda** | 5 | **$10,000** | $10,000 – $15,000 | El techo ($15,000) incluye conocimiento de CONTPAQi. Sr. de soporte supervisión de SOC: $13,000 (1 dato aislado). |
| Supervisor de SOC (referencia) | 1 | $13,000 | — | 1 sola vacante, mezcla monitoreo patrimonial; no generalizar. |

**Estimaciones de mercado (NO son vacantes — marcar como contexto)** `[ESTIMADO]`:
- Salario promedio **soporte técnico** México: **$11,415/mes** (Indeed Career, 3.7k sueldos reportados, actualizado may-2026 — https://mx.indeed.com/career/soporte-t%C3%A9cnico/salaries).
- Salario promedio **técnico/a soporte TI**: **$14,554/mes** (Indeed Career, 690 sueldos, mar-2026 — https://mx.indeed.com/career/t%C3%A9cnico-soporte-ti/salaries).
- Promedio **analista SOC** México: **$24,451/mes** (Jooble, agregado estadístico, 13-may-2026 — https://mx.jooble.org/salary/analista-soc/M%C3%A9xico).
- Rango típico **analista SOC**: $11,167–$31,250 (Glassdoor, 7 sueldos compartidos, 2026; ⚠️ **ambigüedad**: el texto de Glassdoor dice "por año" pero los valores son consistentes con montos mensuales — no usar sin verificar — https://www.glassdoor.com.mx/Sueldos/analista-soc-sueldo-SRCH_KO0,12.htm).
- Distribución de sueldo publicado en OCC para **"analista de soc"** (12 vacantes con monto visible en sept-2026): $10–15k (4), $15–20k (3), $20–30k (2), $30–40k (3) — https://www.occ.com.mx/empleos/de-analista-de-soc/ — consistente con la mediana SOC L1 de ~$18k.

> **Lectura práctica**: el salto de salario real ocurre al pasar de soporte/NOC ($10–18k) a rol SOC/analista de seguridad con 1–2 años de experiencia ($17–35k). El primer rol SOC L1 en CDMX/remoto ronda $18–20k.

---

## 3) Requisitos más repetidos (top 10, n = 26 vacantes core analizadas)

Conteo por vacante (cada vacante cuenta 1 vez si menciona el requisito). Detalle en las ofertas de Computrabajo listadas en el anexo.

| # | Requisito | Vacantes que lo piden | % | Comentario |
|---|---|---|---|---|
| 1 | **Monitoreo continuo** (infraestructura/eventos/plataformas) | 16/26 | 62% | PRTG, SolarWinds, ManageEngine, Nagios/Zabbix mencionados |
| 2 | **Gestión de incidentes / tickets** (triaje, escalamiento, documentación) | 15/26 | 58% | "Incidente" 15; "ticket" explícito en 8 |
| 3 | **Conocimientos de redes** (TCP/IP, OSI, LAN/WAN) | 10–12/26 | 38–46% | "redes" 10; "TCP/IP" explícito 5 |
| 4 | **Trabajo presencial** (en oficina) | 10/26 | 38% | Dominante en SOC/NOC tier-1 |
| 5 | **Windows** (SO y/o servidores) | 7/26 | 27% | Windows Server, Active Directory en algunos |
| 6 | **Turnos** (rotativos/rolados/24/7/nocturno) | 7/26 | 27% | Ver sección 5 |
| 7 | **Certificación** (cualquiera) | 7/26 | 27% | ITIL v4 (4), CCNA (1), CompTIA (1); casi siempre "deseable", no indispensable |
| 8 | **SIEM** | 5/26 | 19% | Splunk, QRadar, Sentinel, Wazuh, FortiSIEM (1 c/u) — raramente exigen una marca |
| 9 | **Inglés** (deseable) | 5/26 | 19% | Se pide más en consultoras/proveedores (Indra, etc.) |
| 10 | **Linux** (básico) | 4/26 | 15% | Aparece en SOC y NOC; nivel básico |
| — | MITRE ATT&CK / NIST CSF | 3/26 | 12% | Solo en perfiles con más seniority (operaciones SOC) |

**Dato relevante**: en estas 26 vacantes, **ninguna exige Security+ de forma obligatoria**; aparece como "deseable" CompTIA ITF+/Security+ (1 vacante, Grupo Pryse). El mercado mexicano junior prioriza **experiencia demostrable (mesa de ayuda/NOC), SIEM conocido y redes**, más que certificaciones. Certs siguen siendo útil para diferenciarse, pero el CV gana con un proyecto/homelab de SIEM (Wazuh) + ticket de incidentes.

---

## 4) Ciudades / mercados con más vacantes y modalidad

Basado en las 28 vacantes recopiladas (sept-2026):

| Mercado | Vacantes | Notas |
|---|---|---|
| **CDMX** (Miguel Hidalgo, Benito Juárez, Tlalpan, Coyoacán, Cuauhtémoc, GAM, Álvaro Obregón) | ~13 | Concentra SOC L1, mesa de ayuda, analistas de seguridad de aseguradoras/bancos (GNP). Zonas: WTC/Benito Juárez y Reforma/Miguel Hidalgo. |
| **Guadalajara (Jalisco)** | 3 | Megacable, FOXCONN GDL, supervisor NOC. |
| **Monterrey (NL)** | 2–3 | Agente NOC Jr, Ingeniero NOC (Integra Soluciones). |
| **Querétaro** | 3 | Analista de ciberseguridad (hasta $35k), supervisor SOC. |
| **Edomex** (Huixquilucan, Naucalpan) | 2 | Monitoreo SOC ($13k), operaciones SOC ($27k). |
| **Hermosillo (Sonora)** | 2 | SOC Jr $25k (7x24) — centro de monitoreo en crecimiento. |
| **Puebla, Cuernavaca, SLP** | 3 | Operador NOC, Analista SOC junior (entry), soporte CONTPAQi. |

**Modalidad (de las 26 core)**:
- **Presencial / esquemas 7x24**: mayoría de SOC L1 y NOC (tan solo 4 lo declaran explícitamente; los demás no lo especifican, pero turnos 24/7 implican oficina). → Ejemplos: Indra (7x24), AXIAN (100% presencial), Sonora (presencial + turnos 3×8), izzi (turnos rolados).
- **Híbrido / remoto**: 5–6 vacantes de analista de ciberseguridad y consultoría (DR Security N1 híbrida; Consultor Ciberseguridad híbrido 2–3 días; Akamai/Indra y analistas de Cuauhtémoc y Querétaro mencionan remoto). El rol SOC L1 100% remoto es **raro**; el híbrido existe sobre todo a partir de analista de seguridad con experiencia.
- El soporte remoto existe como rol (ej. SERTESEG, $12,000/mes — bebee) pero es minoría.

---

## 5) Turnos y condiciones

De las 26 vacantes core, **10 mencionan esquemas de turnos 24/7 / rotativos / nocturnos (≈38%)** — y en SOC/NOC tier-1 la proporción es mucho mayor:

| Vacante | Esquema de turnos reportado |
|---|---|
| Ingeniero SOC Jr N1 (Indra, CDMX) | Modalidad 7x24 |
| Ingeniero/a Monitoreo SOC (Mainbit, Edomex) | turnos + cobertura 24/7 |
| Supervisor SOC (IENTC, Querétaro) | gestión de turnos 24/7 |
| Ingeniero SOC Jr (AIT, Hermosillo) | 7x24, turnos rotativos |
| Analista Ciberseguridad (Sonora) | presencial, turnos rotativos (3 turnos de 8 h) |
| ING JR NOC (izzi, CDMX) | **turnos rolados** 6:00–14:30 / 14:30–22:30 / 22:30–6:30 |
| Ingeniero NOC (Integra, MTY) | turnos rotativos de 12 horas |
| Supervisor Acceso NOC (GDL) | turnos |
| Mesa de control operativa (CDMX, Álvaro Obregón) | **turno nocturno**, 3 días de descanso |

**Condiciones típicas declaradas**: contrato indefinido (ej. Indra), prestaciones de ley + superiores (vales de despensa, fondo de ahorro, SGMM), salarios "libres/nominales". Los turnos rotativos son la norma en NOC/SOC de proveedores de telecom (izzi) y centros de monitoreo; el análisis de alertas en horario nocturno suele pagar igual que diurno en estas vacantes (no se observó diferencial nocturno declarado).

---

## 6) Conclusión: qué perfil piden las vacantes SOC L1 en México hoy

Con base en 5 vacantes SOC L1 + 9 de analista de seguridad + tendencias de NOC/soporte:

1. **Experiencia de entrada**: 6 meses a 2 años en mesa de ayuda / NOC / monitoreo. La puerta de entrada real al SOC no es una certificación, es **experiencia operando tickets y monitoreando** (varias vacantes lo dicen explícitamente, ej. AIT Hermosillo: "experiencia deseable de 1 año en mesa de ayuda").
2. **Conocimientos técnicos que piden (en este orden)**: monitoreo de infraestructura (PRTG/SolarWinds/Zabbix), gestión de incidentes (triaje + escalamiento + documentación), redes TCP/IP/OSI, Windows (+ algo de Linux), y **al menos un SIEM** (Splunk, QRadar, Sentinel, Wazuh o FortiSIEM — cualquiera sirve).
3. **Certificaciones**: útiles pero **no obligatorias** (CompTIA Security+/ITF+, CySA+, ITIL v4, CCNA aparecen como "deseable"). Una cert Security+ + homelab de Wazuh cubre el gap de SIEM que muchas vacantes no explicitan.
4. **Disponibilidad**: presencial y con **disposición a turnos 24/7 rotativos** es la condición más repetida en SOC/NOC tier-1; el trabajo híbrido llega en el salto a analista de seguridad con 1–2 años (sueldos $17–35k).
5. **Salario esperado de primer rol SOC**: $10k (entry recién egresado) a $25k; mediana **~$18k/mes**. Con 1–2 años en analista de seguridad: mediana **~$23k/mes**.

**Perfil CV ganador hoy**: "Soporte TI/NOC con 1 año, experiencia documentada en tickets e incidentes, cursos/homelab SIEM (Wazuh o Splunk), redes TCP/IP, Windows+Linux básico, inglés básico-intermedio, CompTIA Security+ (en curso), disponible para turnos 24/7 en CDMX o remoto".

---

## Anexo: las 28 vacantes recopiladas (con fuente y URL)

*C = Computrabajo (salario publicado por el empleador, mensual);* *B = bebee/Indeed;* *S = SNE-Empleo.gob.mx*

### SOC L1 / monitoreo SOC
| # | Empresa | Puesto | Ciudad | Salario MXN/mes | Modalidad/Turnos | Requisitos clave | URL |
|---|---|---|---|---|---|---|---|
| 1 | Indra Sistemas México | Ingeniero SOC Jr / N1 / 7x24 | Miguel Hidalgo, CDMX | **$20,000** | 7x24 | 6m–2a monitoreo 24/7, SIEM, Palo Alto, licenciatura, tickets | https://mx.computrabajo.com/ofertas-de-trabajo/oferta-de-trabajo-de-ingeniero-soc-jr-n1-7x24-cdmx-en-miguel-hidalgo-E78697597177C52361373E686DCF3405 |
| 2 | Mainbit, S.A. de C.V. | Ingeniero/a Monitoreo - SOC | Huixquilucan, Edomex | **$13,000** | turnos, 24/7 | 1–2 años monitoreo SOC, PRTG/SolarWinds/ManageEngine, redes LAN/WAN, TCP/IP | https://mx.computrabajo.com/ofertas-de-trabajo/oferta-de-trabajo-de-ingenieroa-monitoreo-soc-en-huixquilucan-B09CD621C5F4667861373E686DCF3405 |
| 3 | AXIAN | Ing. SOC Jr | Tlalpan, CDMX | **$18,000** | 100% presencial | triaje de eventos, análisis de incidentes, ciberseguridad, tickets | https://mx.computrabajo.com/ofertas-de-trabajo/oferta-de-trabajo-de-ing-soc-jr-en-tlalpan-A644C4B50AFAD0CE61373E686DCF3405 |
| 4 | Grupo Pryse | Analista SOC (entry) | Cuernavaca, Morelos | **$10,000** | n/a | **recién egresados**, FortiSIEM/Wazuh/ELK, TCP/IP, Windows y Linux, NIST CSF/MITRE deseable, CompTIA ITF+/certs deseables | https://mx.computrabajo.com/ofertas-de-trabajo/oferta-de-trabajo-de-analista-soc-en-cuernavaca-0839624518FC1EA361373E686DCF3405 |
| 5 | AIT Vanguardia Tecnológica | Ingeniero SOC Jr | Hermosillo, Sonora | **$25,000** | 7x24, turnos rotativos | redes TCP/IP, DNS/DHCP/VPN, Windows, Linux básico, AD, triage de alertas, 1 año en mesa de ayuda | https://mx.computrabajo.com/ofertas-de-trabajo/oferta-de-trabajo-de-ingeniero-soc-jr-en-hermosillo-7F4C6A198943091A61373E686DCF3405 |

### Analista de seguridad junior (ciber/seguridad de la información)
| # | Empresa | Puesto | Ciudad | Salario MXN/mes | Modalidad/Turnos | Requisitos clave | URL |
|---|---|---|---|---|---|---|---|
| 6 | (confidencial) | Analista de Ciberseguridad – Operaciones SOC | Naucalpan, Edomex | **$27,000** | n/a | 2 años en SOC, SIEM, análisis forense básico, respuesta a incidentes | https://mx.computrabajo.com/ofertas-de-trabajo/oferta-de-trabajo-de-analista-de-ciberseguridad-operaciones-soc-en-naucalpan-de-juarez-366E27E8FFDA5A0D61373E686DCF3405 |
| 7 | (confidencial) | Analista de Ciberseguridad (proyecto 2 años) | Hermosillo, Sonora | **$20,000** | presencial, turnos rotativos 3×8 | ciberseguridad operacional, turnos | https://mx.computrabajo.com/ofertas-de-trabajo/oferta-de-trabajo-de-analista-de-ciberseguridad-en-sonora-proyecto-de-2-anos-en-hermosillo-* |
| 8 | (confidencial) | Analista de Ciberseguridad | Cuauhtémoc, CDMX | **$27,000** | remoto/presencial | ciberseguridad, SIEM, respuesta a incidentes | https://mx.computrabajo.com/ofertas-de-trabajo/oferta-de-trabajo-de-analista-de-ciberseguridad-en-cuauhtemoc-* |
| 9 | (confidencial) | Analista de Ciberseguridad | Querétaro | **$35,000** | remoto/presencial | seniority media; marca el techo del rango junior-2a | https://mx.computrabajo.com/ofertas-de-trabajo/oferta-de-trabajo-de-analista-de-ciberseguridad-ciber-seguridad-en-queretaro-* |
| 10 | FOXCONN GDL | Ingeniero de seguridad de IT | San Pedro Tlaquepaque, Jal. | **$23,000** | n/a | seguridad IT, 3 años | https://mx.computrabajo.com/ofertas-de-trabajo/oferta-de-trabajo-de-ingeniero-de-seguridad-de-it-en-san-pedro-tlaquepaque-* |
| 11 | Indra Sistemas México | Akamai Security & DNS Specialist | Miguel Hidalgo, CDMX | **$20,000** | remoto/presencial | Akamai, DNS, seguridad perimetral | https://mx.computrabajo.com/ofertas-de-trabajo/oferta-de-trabajo-de-akamai-security-y-dns-specialist-ciudad-de-mexico-en-miguel-hidalgo-* |
| 12 | (confidencial) | Analista de Seguridad de la Información – Sector Salud | Coyoacán, CDMX | **$20,000** | n/a | seguridad de la información, 1 año | https://mx.computrabajo.com/ofertas-de-trabajo/oferta-de-trabajo-de-analista-de-seguridad-de-la-informacion-sector-salud-en-coyoacan-* |
| 13 | GNP | Analista de Seguridad de la Información | Coyoacán, CDMX | **$17,000** | n/a | seguridad de la información, aseguradora, 1 año | https://mx.computrabajo.com/ofertas-de-trabajo/oferta-de-trabajo-de-vacante-gnp-analista-de-seguridad-de-la-informacion-en-coyoacan-* |
| 14 | (confidencial) | Consultor Ciberseguridad | Benito Juárez, CDMX | **$27,000** | híbrido (2–3 días oficina) | consultoría en ciberseguridad, ~2 años | https://mx.computrabajo.com/ofertas-de-trabajo/oferta-de-trabajo-de-consultor-ciberseguridad-en-benito-juarez-* |

### NOC / monitoreo de red junior
| # | Empresa | Puesto | Ciudad | Salario MXN/mes | Modalidad/Turnos | Requisitos clave | URL |
|---|---|---|---|---|---|---|---|
| 15 | (confidencial) | Agente de Mesa de Servicio y NOC Jr. | Monterrey, NL | **$13,000** | n/a | tickets, monitoreo de infraestructura crítica (EcoStruxure deseable) | https://mx.computrabajo.com/ofertas-de-trabajo/oferta-de-trabajo-de-agente-de-mesa-de-servicio-y-noc-jr-en-monterrey-B3FB86712EFC3FCD61373E686DCF3405 |
| 16 | izzi (Televisa) | Ing. Jr. NOC | Benito Juárez, CDMX | **$18,604** | **turnos rolados** 6–14:30 / 14:30–22:30 / 22:30–6:30 | monitoreo, incidencias, herramientas de monitoreo, 1 año | https://mx.computrabajo.com/ofertas-de-trabajo/oferta-de-trabajo-de-ing-jr-noc-izzi-telecom-en-benito-juarez-204F6CD5EF50AE3161373E686DCF3405 |
| 17 | Integra Soluciones | Ingeniero NOC | Monterrey, NL | **$18,000** | turnos rotativos 12 h | SolarWinds/PRTG/eSight, infraestructura, **al menos 1 certificación (no deseable)** | https://mx.computrabajo.com/ofertas-de-trabajo/oferta-de-trabajo-de-ingeniero-noc-en-monterrey-D75CF9F28E5958F861373E686DCF3405 |
| 18 | (confidencial) | Supervisor Acceso NOC | Guadalajara, Jal. | **$13,000** | turnos | supervisión de acceso NOC | https://mx.computrabajo.com/ofertas-de-trabajo/oferta-de-trabajo-de-supervisor-acceso-noc-en-guadalajara-688D5CE360718FAA61373E686DCF3405 |
| 19 | Servicel Servicios Móviles | Operador NOC | San Andrés Cholula, Puebla | **$12,000** | remoto/presencial | LAN/WAN/MAN, OSI, TCP/IP, troubleshooting N1-N2 | https://mx.computrabajo.com/ofertas-de-trabajo/oferta-de-trabajo-de-operador-noc-en-san-andres-cholula-FA25D765FD45AD4261373E686DCF3405 |
| 20 | Megacable | Ingeniero de servicios interactivos Jr. | Guadalajara, Jal. | **$15,000** | n/a | monitoreo video digital, incidentes N1, redes/middleware | https://mx.computrabajo.com/ofertas-de-trabajo/oferta-de-trabajo-de-ingeniero-de-servicios-interactivos-jr-en-guadalajara-98BE55898BDD7BF161373E686DCF3405 |

### Soporte TI / mesa de ayuda
| # | Empresa | Puesto | Ciudad | Salario MXN/mes | Modalidad/Turnos | Requisitos clave | URL |
|---|---|---|---|---|---|---|---|
| 21 | DR Security | Mesa de Ayuda N1 Jr | Miguel Hidalgo, CDMX | **$14,000** | híbrida | **certificación ITIL v4 (requerida)**, ITSM/Jira, gestión de incidentes | https://mx.computrabajo.com/ofertas-de-trabajo/oferta-de-trabajo-de-mesa-de-ayuda-n1-jr-en-miguel-hidalgo-4B32A0E77EAFAC5F61373E686DCF3405 |
| 22 | Dcloud Transformation | Mesa de Ayuda Soporte Técnico (WTC) | Benito Juárez, CDMX | **$10,000** | presencial | mantenimiento equipos (impresoras, escáner), configuración de apps | https://mx.computrabajo.com/ofertas-de-trabajo/oferta-de-trabajo-de-mesa-de-ayuda-soporte-tecnico-wtc-mexicobenito-juarez-en-benito-juarez-F2112D806611861161373E686DCF3405 |
| 23 | (confidencial) | Mesa de control operativa (3 días descanso) | Álvaro Obregón, CDMX | **$10,000** | **turno nocturno** | monitoreo/control operativo nocturno | https://mx.computrabajo.com/ofertas-de-trabajo/oferta-de-trabajo-de-mesa-de-control-operativa-3-dias-de-descanso-en-alvaro-obregon-* |
| 24 | (confidencial) | Mesa de ayuda o control – seguimiento técnico crítico | Álvaro Obregón, CDMX | **$10,000** | n/a | seguimiento técnico crítico | https://mx.computrabajo.com/ofertas-de-trabajo/oferta-de-trabajo-de-mesa-de-ayuda-o-control-seguimiento-tecnico-critico-en-alvaro-obregon-* |
| 25 | Contigo Consultores | Soporte Técnico TI y CONTPAQi | San Luis Potosí | **$15,000** | presencial | Windows, Windows Server, SQL Server, CONTPAQi, equipos de cómputo | https://mx.computrabajo.com/ofertas-de-trabajo/oferta-de-trabajo-de-soporte-tecnico-ti-y-contpaqi-tiempo-completo-en-san-luis-potosi-E7CAD8948A8975D861373E686DCF3405 |

### Referencias externas (vacantes concretas de otras fuentes)
| # | Fuente | Puesto | Ciudad | Salario | Notas | URL |
|---|---|---|---|---|---|---|
| 26 | IENTC (C) | Supervisor de SOC – Seguridad y monitoreo | Querétaro | **$13,000** | 24/7; mezcla monitoreo patrimonial/CCTV; referencia de supervisión | https://mx.computrabajo.com/ofertas-de-trabajo/oferta-de-trabajo-de-supervisor-de-soc-seguridad-y-monitoreo-en-queretaro-3AE660EED767008461373E686DCF3405 |
| 27 | Headhunters TI (bebee/Indeed) | Ing. de soporte técnico | Lindavista (GAM), CDMX | **$18,000 neto** | full-time, presencial; publicada 11-sep-2026; origen LinkedIn/Indeed | https://bebee.com/mx/jobs/role/tecnico-en-soporte-remoto (listado originado en Indeed/Talenteca) |
| 28 | SNE – Empleo.gob.mx | Auxiliar de Soporte TI | (vacante federal) | **no reportado** ("Sueldo 100% nominal") | instalación/actualización de SO, soporte a usuarios y hardware | https://www.empleo.gob.mx/puesto-de-trabajo/vacante/20485050-AUXILIAR-DE-SOPORTE-TI |

\* URL acortada: el sufijo de la oferta original (`-<HEX>`) se omitió en las filas con `*`; la vacante es localizable en Computrabajo MX buscando el título exacto + empresa/ciudad indicados. Las filas 1–5, 15–25 y 26 llevan la URL canónica completa extraída de la oferta.

---

## Limitaciones de este análisis

1. **Muestra pequeña y sesgada a lo publicado**: 28 vacantes (26 con sueldo) capturadas el 16-sep-2026; Computrabajo publica ~24 ofertas por página resultado y muchas vacantes (especialmente vía reclutadores/confidenciales) no declaran sueldo ("Sueldo no mostrado por la empresa", p. ej. en OCC).
2. **Posible sesgo geográfico**: el listado inicial de "soc"/"monitoreo" de Computrabajo sobre-representa CDMX y el centro del país; plazas regionales (Monterrey cara a cara, Bajío industrial) pueden diferir.
3. **Los salarios publicados son list price del empleador** (bruto/nominal): no incluyen prestaciones superiores ni vales, el dato neto puede ser 10–15% menor; además no se capturó negociación real (Glassdoor) salvo para analista SOC (n=7, unidades ambiguas).