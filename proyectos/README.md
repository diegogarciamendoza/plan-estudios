# Proyectos

**Esta carpeta está vacía a propósito.** Aquí van las **prácticas técnicas reproducibles**: algo que
otra persona puede descargar, ejecutar y comprobar. Todavía no hay ninguno, y prefiero dejarlo
declarado antes que llamar "proyecto" a un certificado o a una actividad de curso.

## Qué va a ir aquí (fase 2 del plan, meses 3–6)

| Proyecto | Qué incluye | Estado |
|---|---|---|
| Investigación de fuerza bruta | dataset/registro, consulta de fallos de autenticación, umbral justificado, falsos positivos, timeline, informe de 1 página | ⬜ no iniciado |
| Detección de PowerShell sospechoso | Event IDs, Sysmon, consulta SIEM, caso benigno vs. sospechoso, mapeo MITRE ATT&CK | ⬜ no iniciado |
| Análisis de phishing | cabeceras, dominio/URL, SPF/DKIM/DMARC, IOC, respuesta recomendada, ticket simulado | ⬜ no iniciado |

Cada uno con: README, arquitectura, pasos de reproducción, consultas, capturas, resultados,
**falsos positivos**, "qué haría después" y aviso de laboratorio.

## Idea declarada (2026-09-30, sin fecha)

**Laboratorio en Docker con ejercicios creados por mí y autoevaluables**: un entorno tipo
*OverTheWire Bandit*, pero con **scripts que califican si el trabajo se realizó correctamente**
(comprobaciones sobre el estado del sistema, no sobre texto pegado). Se diseña cuando lleguen los
cursos 4 (Linux y SQL), 6 (detección) y 7 (Python) — no antes: necesita esas tres piezas.

Sería a la vez material de repaso propio y una pieza de portafolio inspeccionable por un tercero.

## Regla

Un proyecto aquí tiene que poder **ejecutarse o inspeccionarse** por alguien que no sea yo. Si no,
es una nota de estudio y va al diario o a `cursos/`.
