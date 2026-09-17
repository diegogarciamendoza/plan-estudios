---
tipo: tema
dia_plan: 01
fecha: 2026-09-17
modulo: M1-fundamentos
estado: ✅ hecho
tags: [shell, linux, comandos]
enlaces:
  - "diario/2026-09-17"
  - "M1-fundamentos/dia01-lab-shell"
---

# Día 1 · Tema — Comandos básicos de Shell

## ¿Qué aprendí?

- **`pwd` / `ls` / `cd`**: navegación con rutas relativas y absolutas. `cd` sin argumentos vuelve a `~`; `..` es el directorio padre.
- **`ls` "ver todo"**: `-l` detalle, `-a` incluye ocultos, `-h` tamaños humanos. Uso diario: `ls -lah`.
- **`cat` vs `less`**: `cat` concatena/muestra (para cortos); `less` pagina (para largos). Atajos: `Espacio` (página), `g`/`G` (inicio/fin), `/` (buscar), `q` (salir).
- **Redirección**: `>` crea/sobreescribe, `>>` añade al final. `cat a b > c` concatena dos archivos en uno nuevo.
- **`man`**: manual paginado (usa `less` internamente) — consultar sintaxis siempre que olvide un comando.

## El "por qué" (lo que separa conocer de entender)

- **`less` sobre `cat`** para archivos largos: `cat` escupe TODO en pantalla y solo ves el final; `less` pagina y deja leer a tu ritmo. La elección importa más que el comando en sí.
- **`>` vs `>>`**: el primero sobreescribe, el segundo preserva lo existente y añade. Elegir mal borra trabajo.

## 1 ejemplo conceptual

```bash
ls -lh /var/log      # tamaños humanos + detalle del directorio de logs
man grep             # consultar opciones de grep (paginado, sale con q)
```

## Dudas pendientes

- Ninguna por ahora. Próximo del plan: `find`, `grep` y pipes (`|`).

## Vocabulario nuevo (en inglés)

| Término | Significado |
|---|---|
| recursive | operación que también entra a subdirectorios (ej. `ls -R`, `-r`) |
| human-readable | tamaño legible para personas (`ls -h`: KB/MB/GB) |
| append | añadir al final sin borrar (`>>`), vs `>` que sobrescribe |