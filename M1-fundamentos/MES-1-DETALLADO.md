# Mes 1 — Fundamentos de SOC (semana a semana)

> Para Diego. En español, directo. Fuente: `~/wiki/concepts/plan-carrera-ciberseguridad.md` (v3).
> Resumen general del plan: [`GENERAL.md`](./GENERAL.md)

## Cómo usar este documento

- Cada semana = teoría (8 h) + laboratorio (8 h) + documentación (2 h) + inglés/empleo (2 h) = **20 h**.
- Todo lo que hagas se guarda en tu repo Git (ver Semana 1). Si no está en el repo, no está hecho.
- Se atrasó algo? Prioridad: **cert Google ≥ labs básicos ≥ inglés**. El inglés es lo primero que se abandona — no lo atrases.

## Base del mes: Google Cybersecurity Certificate (Coursera Plus)

- **URL**: <https://www.coursera.org/professional-certificates/google-cybersecurity>
- **Cubre**: Linux, Python, SQL, SIEM, logs e incident response. **~170 h en total** (9 cursos — ver el mapa).
- **Mes 1 = la primera parte** (el certificado completo abarca meses 1–2). No intentes terminarlo este mes; el objetivo es la base.
- **Ritmo**: ~8 h/semana de teoría salen del certificado; los laboratorios paralelos fijan lo que ves ahí.

### Mapa del certificado (verificado 2026-09-19, **re-verificado 2026-09-22** en coursera.org)

**9 cursos** (~170 h de contenido técnico + el módulo de carrera). El avance se cuenta así: **cursos completados / 9** y, dentro de cada curso, sus **módulos** (el Curso 1 tiene 4). La credencial de Google se emite al completar los 9 cursos.

> ⚠️ **Cambio 2026-09-22:** el programa pasó de 8 a **9 cursos**. La plataforma ya muestra `Course 1 of 9` y el HTML oficial de Coursera lista el 9.º: *Accelerate Your Job Search with AI* (búsqueda de empleo, no técnico). Los 8 títulos anteriores no cambiaron.

| # | Curso | Estado |
|---|---|---|
| 1 | Foundations of Cybersecurity *(4 módulos)* | ✅ **completado 2026-09-22** — `Grade: 90.63%` · *Module 4 challenge* **94.44%** · certificado verificado |
| 2 | Play It Safe: Manage Security Risks | ⬜ |
| 3 | Connect and Protect: Networks and Network Security | ⬜ |
| 4 | Tools of the Trade: Linux and SQL | ⬜ |
| 5 | Assets, Threats, and Vulnerabilities | ⬜ |
| 6 | Sound the Alarm: Detection and Response | ⬜ |
| 7 | Automate Cybersecurity Tasks with Python | ⬜ |
| 8 | Put It to Work: Prepare for Cybersecurity Jobs | ⬜ |
| 9 | Accelerate Your Job Search with AI *(módulo de carrera, añadido 2026)* | ⬜ |

## Recursos del mes (gratis o ya pagados)

| Recurso | URL | Para qué |
|---|---|---|
| Google Cybersecurity Certificate | <https://www.coursera.org/professional-certificates/google-cybersecurity> | Esqueleto del mes (Coursera Plus patrocinado) |
| Cisco Networking Academy | <https://www.netacad.com> | Redes; portal gratis self-paced: <https://www.skillsforall.com> (ahí también se descarga Packet Tracer gratis) |
| Prof. Messer (YouTube) | <https://www.professormesser.com> | Repasos Network+ / Security+ en video |
| The Linux Command Line (W. Shotts) | <https://linuxcommand.org/tlcl.php> | PDF oficial gratis de línea de comandos Linux |
| OverTheWire — Bandit | <https://overthewire.org/wargames/bandit/> | Práctica de shell por niveles |
| Microsoft Learn | <https://learn.microsoft.com> | Docs oficiales Windows (buscar "Windows security auditing") |
| MITRE ATT&CK | <https://attack.mitre.org> | Matriz de tácticas/técnicas (intro) |
| Wireshark docs + capturas de muestra | <https://www.wireshark.org/docs/> · <https://wiki.wireshark.org/SampleCaptures> | Aprender y practicar con pcaps reales |
| MDN — Glossary: TLS | <https://developer.mozilla.org/en-US/docs/Glossary/TLS> | Definición precisa de TLS/SSL en inglés técnico sencillo (1 min) |
| MDN — Transport Layer Security | <https://developer.mozilla.org/en-US/docs/Web/Security/Transport_Layer_Security> | Referencia de facto de la web: handshake, certificados, versiones |
| How HTTPS works (DNSimple) | <https://howhttps.works/> | Cómic visual y preciso: el handshake paso a paso |
| RFC 9846 — TLS 1.3 (julio 2026) | <https://datatracker.ietf.org/doc/html/rfc9846> | Fuente **autoritativa y vigente**: obsoleta el RFC 8446 (y el 5246, TLS 1.2). Para consultar, no leer entera |

### DNS — fuentes para profundizar (cuando toque, no hoy)

| Fuente | URL | Para qué |
|---|---|---|
| How DNS works (DNSimple) | <https://howdns.works/> | Cómic visual: qué pasa entre escribir un dominio y ver la página |
| DNS for Rocket Scientists (Zytrax) | <https://www.zytrax.com/books/dns/> | Referencia gratis con **formato de zona** y todos los tipos de registro |
| RFC 1035 | <https://datatracker.ietf.org/doc/html/rfc1035> | El estándar: §3.3 formato de cada RR (incluido MX), §5 formato de zona (*master files*) |
| Cloudflare Learning — DNS | <https://www.cloudflare.com/learning/dns/what-is-dns/> | Explicación clara y visual (su WAF bloquea lectores automáticos: ábrela en el navegador) |
| Prof. Messer — Network+ N10-009 | <https://www.professormesser.com/network-plus/n10-009/> | Video de DNS/HTTP, ya en el plan |
| Práctica | `dig MX gmail.com +short` (paquete `dnsutils`) o DoH: `curl -H 'accept: application/dns-json' 'https://cloudflare-dns.com/dns-query?name=gmail.com&type=MX'` | Consultar registros reales sin instalar nada |

---

## Semana 1 — Arranque: cert + redes base + shell + Git

### Teoría (8 h)
- [ ] Cert Google Curso 1 (Foundations of Cybersecurity): qué es un SOC, dominios de seguridad, marcos de trabajo, ética — primera mitad.
- [ ] Redes base: modelo TCP/IP vs OSI, flujo de un paquete por la red; DNS (qué resuelve, registros básicos); HTTP/HTTPS y TLS en 5 ideas (handshake resumido).
- [ ] Ver 1–2 videos de Prof. Messer de Network+ sobre TCP/IP y DNS si algo no quedó claro.

### Laboratorio (8 h)
- [ ] Shell Linux: `pwd, ls, cd, cat, less, man, touch, mkdir, cp, mv, rm` — practicar hasta no mirar las notas.
- [ ] OverTheWire **Bandit niveles 0–5**.
- [ ] Git + Markdown: crear repo `plan-estudios` en GitHub, subir este plan y tu carpeta de notas; **commit cada día que estudies**.
- [ ] Primer README.md con tu contexto y objetivo (en tu propio markdown, practicando formato).

### Documentación (2 h)
- [ ] Estructura de tu carpeta de estudio: `diario/` + `M1-fundamentos/` (todo plano, con prefijo `lab-` / `entregable-`).
- [ ] Plantilla de nota de estudio (tema → qué aprendí → 1 ejemplo práctico).

### Inglés aplicado a SOC (2 h)
- [ ] Glosario SOC parte 1 (20 términos): *threat, vulnerability, incident, alert, triage, log, SIEM, false positive, IOC, phishing, malware, exploit, authentication, authorization, firewall, IDS/IPS, endpoint, malware analyst, incident response, playbook* — con tu definición de 1 línea en inglés.
- [ ] Leer en voz alta la intro de MITRE ATT&CK (<https://attack.mitre.org>) y anotar 5 palabras nuevas.

### Entregables de la semana
- [ ] Coursera Plus activo y Curso 1 en marcha.
- [ ] Bandit niveles 0–5.
- [ ] Repo Git con primeros commits.
- [ ] Glosario de 20 términos.

---

## Semana 2 — Redes un nivel más + Windows y Event Viewer

### Teoría (8 h)
- [ ] Cert Google, curso de redes (Connect and Protect): conceptos de red, firewall, VPN — a tu ritmo.
- [ ] **VLAN, NAT y routing básico**: qué aísla una VLAN, cómo NAT saca tráfico a internet, para qué sirve una tabla de rutas.
- [ ] **Windows/AD a nivel alto** (por qué el corporativo mexicano es mayormente Windows) y diferencia entre Security log y System log.

### Laboratorio (8 h)
- [ ] **Packet Tracer** (gratis vía NetAcad/SkillsForAll): topología casa/oficina con router + switch, 2 VLAN y NAT. Guardar el archivo `.pkt`.
- [ ] **Event Viewer**: abrir Registro de seguridad (Security log), explorar qué eventos hay y de qué tipo.
- [ ] Aprender a identificar en el log: **4624** (inicio de sesión correcto), **4625** (fallo de inicio de sesión), **4672** (privilegios especiales), **4688** (creación de proceso).
- [ ] Generar un 4625 a propósito: intentar iniciar sesión con contraseña incorrecta y encontrarlo en el log.
- [ ] PowerShell: documentar los **primeros 5 comandos** (ej. `Get-WinEvent`, `Select-Object`, `Where-Object`, `Format-List`, `Get-Service`) con ejemplo y salida en tu repo.
- [ ] Linux: `dig`/`nslookup` para resolver dominios y ver respuestas DNS.

### Documentación (2 h)
- [ ] **Mapa de red v1** del lab dibujado (drawio o texto) explicando VLAN, NAT y rutas. Se refina la semana 4.

### Inglés aplicado a SOC (2 h)
- [ ] Vocabulario semana 2: *logon, logoff, failed attempt, valid credentials, privilege escalation, network segment, routing, authentication*.
- [ ] Leer el doc oficial de Microsoft sobre el evento **4625** (buscar en learn.microsoft.com "security event 4625") en inglés; anotar 3 facts de la descripción.

### Entregables de la semana
- [ ] Topología Packet Tracer + mapa de red v1 explicado.
- [ ] 5 comandos PowerShell documentados (con salida real).
- [ ] Encontrar en tu Windows un evento 4625 real (el que generaste).

---

## Semana 3 — Linux shell a fondo + SQL + Python

### Teoría (8 h)
- [ ] Cert Google, curso Linux y SQL: shell, filtros (`grep`), permisos, usuarios.
- [ ] SQL: `SELECT, WHERE, ORDER BY, GROUP BY, JOIN` (a nivel básico, con ejemplos).
- [ ] Python: sintaxis básica (variables, listas, `for/if`, leer archivos).

### Laboratorio (8 h)
- [ ] **The Linux Command Line** (Shotts, PDF): caps. 1–6 practicados.
- [ ] Leer logs en Linux: `/var/log/auth.log` (o `journalctl`), `grep "Failed"` para ver intentos de login fallidos.
- [ ] **SQLite**: crear tabla `logins` con datos de prueba (usuario, IP, hora, éxito/fallo) y escribir **10 consultas** (fallos por IP, usuarios con más intentos, ventana de tiempo, etc.).
- [ ] **Python**: script que abre un archivo de log, cuenta líneas con "Failed" y muestra el top 5 de IPs. (Es el germen del proyecto de fuerza bruta del mes 3 — guardarlo.)
- [ ] Completar los **5 comandos PowerShell restantes** (total 10) documentados en el repo.

### Documentación (2 h)
- [ ] Documento `M1-fundamentos/entregable-10-consultas-sql.md`: pregunta → consulta → resultado (con las 10).

### Inglés aplicado a SOC (2 h)
- [ ] Vocabulario semana 3: *query, filter, correlate, baseline, anomaly, brute force, enumeration, permissions, privilege*.
- [ ] Leer una página de docs de Linux/SQL en inglés (ej. de Microsoft Learn) y resumirla en 3 oraciones en inglés.

### Entregables de la semana
- [ ] 10 consultas SQL documentadas.
- [ ] Script Python que cuenta fallos de login (funcionando).
- [ ] 10 comandos PowerShell documentados (total del mes ✅).

---

## Semana 4 — Wireshark + MITRE ATT&CK + SIEM intro + CV

### Teoría (8 h)
- [ ] Cert Google, cursos de detección/respuesta (Sound the Alarm): qué es un **SIEM**, ciclo de **incident response**, idea de triage — empezar.
- [ ] **MITRE ATT&CK intro**: matriz, táctica vs técnica, grupos de tácticas. Ejemplos: T1078 (Valid Accounts), T1059 (Command and Scripting Interpreter).

### Laboratorio (8 h)
- [ ] **Wireshark**: instalar, capturar tu propia navegación; filtrar por `dns`, `tcp`, `http`; seguir un stream HTTP completo.
- [ ] Ver el **handshake TLS** en una captura (ClientHello / ServerHello / cambio de claves) — solo identificar los paquetes.
- [ ] Descargar una captura de muestra de Wireshark SampleCaptures y analizarla: qué protocolos hay (Estadísticas → Protocol Hierarchy).
- [ ] Mapear **1 técnica de MITRE** que hayas observado en tus logs/capturas (ej. fuerza bruta ≈ T1110) en tu nota.

### Documentación (2 h)
- [ ] **Investigación básica con Wireshark**: captura + 3 hallazgos + conclusión (1 página) en `M1-fundamentos/` (prefijo `entregable-`).
- [ ] Terminar el **mapa de red final** con lo aprendido de VLAN/NAT/DNS.

### Empleo (parte de las 2 h de esta semana)
- [ ] **Primer CV técnico**: transición técnica con experiencia previa (resolución de problemas, reparación, autonomía, disciplina) — sin ocultar la edad ni hacerla el centro.
- [ ] LinkedIn al día (foto, sector, una línea de objetivo).

### Inglés aplicado a SOC (2 h)
- [ ] **Primer resumen ejecutivo en inglés** de tu investigación de Wireshark (5–8 líneas: qué pasó, qué encontré, qué recomiendo).
- [ ] Grabarte 90 s: "What is your background and why cybersecurity?" — escucharte y repetir hasta que suene natural.

### Entregables de la semana
- [ ] Investigación Wireshark de 1 página + resumen ejecutivo en inglés.
- [ ] Mapa de red final explicado.
- [ ] Primer CV técnico + LinkedIn al día.

---

## Entregables de fin de mes (checklist global)

- [ ] **Mapa de red explicado** (VLAN, NAT, routing, DNS) — v1 en semana 2, final en semana 4.
- [ ] **10 consultas SQL** documentadas (pregunta → consulta → resultado).
- [ ] **10 comandos PowerShell** documentados con salida real.
- [ ] **Investigación básica con Wireshark** (captura + 3 hallazgos + conclusión, 1 página).
- [ ] **Primer CV técnico** + LinkedIn al día.
- [ ] Cert Google: primera parte completada (cursos iniciales del mes 1).
- [ ] Repo `plan-estudios` con commits regulares y todos los entregables versionados.

## Inglés aplicado a SOC (módulo transversal, 2 h/sem)

Objetivo: inglés **útil para el trabajo**, no curso general.

- **Escribir**: un resumen ejecutivo en inglés por cada investigación del portafolio (el primero: semana 4).
- **Leer**: documentación oficial en inglés (Microsoft, Cisco, Elastic — <https://www.elastic.co/docs>) y extraer 3 facts por lectura.
- **Vocabulario**: glosario SOC propio, 20 términos por semana (los de cada semana quedan anotados arriba).
- **Hablar (desde mes 2)**: preguntas de entrevista técnica en inglés, grabadas y reescuchadas.

## Notas

- Precios/salarios no verificados aquí: ver `GENERAL.md` (Security+ ~$7,300–7,500 MXN; presupuesto anual ~$7,500–9,000 MXN).
- URLs de cursos específicos dentro de Coursera/Microsoft Learn pueden cambiar: si un enlace profundo falla, buscar por nombre ("Google Cybersecurity Certificate", "Windows security event 4625") — el contenido es el mismo.