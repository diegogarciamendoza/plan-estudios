# Entregables

**Qué es un entregable aquí:** un trabajo propio que **un tercero puede leer y evaluar sin contexto
del curso** — con su alcance, su método, sus límites y lo que *no* demuestra. No es una tarea del
curso, no es un certificado y no es una nota personal.

**Regla anti-relleno:** si un curso no produjo algo mostrable, se escribe **"ninguno"**. No se
inventa material para llenar la carpeta.

## Índice

| Trabajo | Curso / origen | Estado | Qué no pretende demostrar |
|---|---|---|---|
| Evaluación de controles de seguridad | Google C02 · *Portfolio Activity* | 🟡 **existe** (calificado **100%**), pendiente de reformatear a formato propio | auditoría de una organización real |
| Respuesta a un incidente con el marco NIST | Google C03 · *Portfolio Activity* | 🟡 **existe** (calificado **100%** el 2026-10-07), pendiente de reformatear a formato propio | respuesta real a un incidente |
| Investigación de mercado laboral (México) | Trabajo propio (2026-09-16) | ✅ terminada — [informe](../vacantes-analisis.md) · [versión remota global](../vacantes-remoto-global.md) | garantía de empleo o de salario |
| Glosario SOC en inglés | Trabajo propio, transversal | ✅ en curso (56+ términos) — [glosario](../glosario.md) | dominio del inglés hablado |
| Professional statement | Google C01 · *Portfolio Activity* | ⬜ **en evaluación** (decisión pendiente de Diego) | experiencia laboral real |
| Proyectos técnicos reproducibles | Fase 2 del plan | ⬜ no iniciados — [proyectos/](../proyectos/README.md) | experiencia de producción |

## Estructura de un entregable

Cada entregable lleva, como mínimo:

```markdown
## Alcance            (qué cubre y qué queda fuera)
## Contexto y supuestos
## Método             (cómo se hizo, con qué fuentes)
## Hallazgos          (numerados: H-001, H-002…)
## Límites de la evidencia   (lo que NO puedo afirmar con esto)
## Qué mejoraría      (siguiente iteración)
```

En la priorización se usa **impacto** (bajo/medio/alto) y **confianza** (baja/media/alta) con su
base declarada (*supuesto del escenario · evidencia proporcionada · evidencia ausente*). **No** se
usan puntuaciones numéricas de probabilidad sin metodología defendible.

## Por qué `entregables/` está separado de `cursos/`

`cursos/` es el **estado** (dónde voy en cada curso). `entregables/` es el **trabajo producido**
(qué puedo mostrar). Un archivo puede aparecer en los dos, pero con contenidos distintos: en el
tracker, el enlace; aquí, el trabajo.

## Cómo se publica

1. Se escribe primero el borrador (puede ser feo y estar a medias).
2. Se le añaden las secciones de **límites** y **qué mejoraría**.
3. Se revisa que no haya material de terceros (transcripciones, lecturas, quizzes de Coursera).
4. Solo entonces se enlaza desde el [README](../README.md).
