---
tipo: hoja-modulo
curso: C03
modulo: M03
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

# C03 · M03 — Secure against network intrusions

> **Curso 3 *Connect and Protect: Networks and Network Security* · módulo 03 de 04.** Duración: la muestra la plataforma.
> Se abre el día que **empieza** el módulo (2026-10-07) y se cierra el día que apruebas su *module challenge*.
> Una hoja = un módulo. Nunca un resumen por curso (el motivo está en [[repaso/README]]).

**Cómo se usa (3 reglas):**

1. **Se responde, no se lee.** La respuesta vive dentro de un callout plegado `> [!success]-`: primero la dices/escribes de memoria, **después** la destapas.
2. **Aquí no entra contenido del curso.** El *mapa* cita la lección (para saber de dónde sale); lo demás son **tus palabras** en español + tus términos en inglés. Nada de pegar transcripts: el repo es público y el material de Coursera vive fuera ([[MES-1-DETALLADO]] → *cómo obtenerlo*).
3. **Se llena mientras estudias**, no al final de golpe: la lección que cierras hoy deja su fila y su pregunta hoy.

**Hecho cuando:** *module challenge* **≥80%** + mapa completo (todas las lecciones) + **los 14 términos del módulo producidos en inglés** (dichos en voz alta *y* escritos) + fuentes marcadas.

## En una frase

> ¿Qué problema del trabajo real resuelve este módulo? (una frase tuya, sin copiar)

## Mapa del módulo

*Nombres reales de las lecciones, leídos del export del curso el 2026-10-07 (orden del export; el de la plataforma puede variar).*

| # | Lección (nombre real) | Qué me llevo (1 línea, mía) |
|---|---|---|
| 1 | Welcome to module 3 | |
| 2 | How intrusions compromise your system | |
| 3 | The case for securing networks | |
| 4 | Read tcpdump logs | |
| 5 | Real-life DDoS attack | |
| 6 | Denial of Service (DoS) attacks | |
| 7 | Overview of interception tactics | |
| 8 | Malicious packet sniffing | |
| 9 | IP Spoofing | |
| 10 | Activity: *Analyze network layer communication* (con ejemplar) | |
| 11 | Activity: *Analyze network attacks* (con ejemplar) | |
| 12 | Glossary terms from module 3 | |
| 13 | Wrap-up | |
| — | *Vídeo de rol*: Matt — A professional on dealing with attacks | |

> ⚠️ El export trae el **ejemplar** de las dos actividades, no el enunciado calificado: al llegar a ellas, apunta en la nota del día si son **calificadas** (`Submitted · Graded`) y su porcentaje. Si producen un *Cybersecurity incident report*, ese informe es **entregable del portafolio** (se reformatea al formato propio, no se pega la plantilla).

## Recuperación (decir de memoria, después destapar)

**1. *Passive* vs *active packet sniffing*: ¿en qué se diferencian y por qué la variante pasiva es casi un recuerdo de la era del hub?**
> [!success]- Mi respuesta
> _(dila en voz alta y escríbela aquí; si te trabas, anótalo — el bloqueo es el dato)_

**2. DoS vs DDoS: qué cambia entre uno y otro y por qué el segundo es más difícil de filtrar. Nombra 3 variantes de este módulo (SYN flood, ICMP flood, ping of death, smurf) y di qué tienen en común.**
> [!success]- Mi respuesta
> _(la pregunta de *cuál y por qué* es la que más te saltas: respóndela escrita, no mental)_

**3. *On-path attack*, *IP spoofing* y *replay attack*: ¿qué necesita el atacante en cada uno y en qué momento del viaje del paquete actúa?**
> [!success]- Mi respuesta
> _(transferencia: si los tres te suenan a "robar el paquete", sepáralos por el momento y por lo que requiere cada uno)_

**4. Lee esto como lo leería un analista y di qué ataque ves: ráfaga de paquetes `ICMP echo request` a un destino con la **IP de origen de la víctima** y sin respuesta en el otro extremo.**
> [!success]- Mi respuesta
> _(es la pregunta que te va a hacer un *module challenge*: dato → ataque → una mitigación)_

## Inglés — producción del módulo

Los términos son los **14 del glosario del módulo** (lección *Glossary terms from module 3*); se cierran **diciéndolos de memoria en voz alta y escribiéndolos**: si el término se produce mal (forma, acrónimo, artículo), va a tarjeta SRS.

| # | Término (EN) | Lo dije en voz alta | Lo escribí | Una frase mía usándolo |
|---|---|---|---|---|
| 1 | Active packet sniffing | | | |
| 2 | Botnet | | | |
| 3 | Denial of service (DoS) attack | | | |
| 4 | Distributed denial of service (DDoS) attack | | | |
| 5 | ICMP flood | | | |
| 6 | Internet Control Message Protocol (ICMP) | | | |
| 7 | IP spoofing | | | |
| 8 | On-path attack | | | |
| 9 | Packet sniffing | | | |
| 10 | Passive packet sniffing | | | |
| 11 | Ping of death | | | |
| 12 | Replay attack | | | |
| 13 | Smurf attack | | | |
| 14 | Synchronize (SYN) flood attack | | | |

## Fuentes

Solo fuentes **públicas y verificadas** (fecha de verificación incluida). El mapa de todas las del plan vive en [[repaso/README]].

| Fuente | Qué cubre de este módulo | Verificada |
|---|---|---|
| <https://attack.mitre.org/techniques/T1498/> | **Network DoS** en el lenguaje de un SOC (aquí vive el *direct network flood*) | ✅ HTTP 200 · 2026-10-07 |
| <https://attack.mitre.org/techniques/T1040/> | **Network Sniffing** (pasivo/activo tal como lo mapea ATT&CK) | ✅ HTTP 200 · 2026-10-07 |
| <https://attack.mitre.org/techniques/T1557/> | **Adversary-in-the-Middle**: el nombre actual de *on-path attack* | ✅ HTTP 200 · 2026-10-07 |
| <https://www.rfc-editor.org/rfc/rfc792.html> | ICMP — el protocolo detrás de *ping of death*, *smurf* e *ICMP flood* | ✅ HTTP 200 · 2026-10-07 |
| <https://www.rfc-editor.org/rfc/rfc9293.html> | TCP — la especificación vigente (obsoleta la 793) para el *SYN flood* | ✅ HTTP 200 · 2026-10-07 |
| <https://www.tcpdump.org/manpages/tcpdump.1.html> | Manual de `tcpdump`: leer los logs de la lección *Read tcpdump logs* | ✅ HTTP 200 · 2026-10-07 |

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
