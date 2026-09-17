# Lab 1 — Fundamentos de Shell

> Día 1 · pwd, ls, cd, cat, less, man · evaluado 2026-09-17

## ¿Qué aprendí?

- **`pwd` / `ls` / `cd`**: navegación con rutas relativas y absolutas. `cd` sin argumentos vuelve a `~`; `..` es el directorio padre.
- **`ls` con flags para "ver todo"**: `-l` detalle, `-a` incluye ocultos, `-h` tamaños humanos. Uso diario: `ls -lah`.
- **`cat` vs `less`**: `cat` concatena/muestra (para archivos cortos); `less` pagina (para largos). `less` usa espacio (página), `g`/`G` (inicio/fin), `/` (buscar), `q` (salir).
- **Redirección**: `>` sobreescribe/crea, `>>` añade al final. `cat a b > c` concatena dos archivos en uno nuevo.
- **`man`**: manual paginado (usa `less` internamente) — consulto sintaxis y opciones cuando olvido un comando.

## 1 ejemplo práctico

Creé `combinado.txt` concatenando dos archivos con redirección a archivo nuevo:

```bash
cat notas.txt README.md > combinado.txt
cat combinado.txt   # verificar: ambas contenidos, 6 líneas
```

## Matices que me marcaron en la revisión

1. **`ls -h`**: sin `-h` los tamaños van en bytes brutos (`5000000`); con `-h` se leen humanos (`4.8M`). En un `ls -l` de disco completo, los bytes son ilegibles → `ls -lh` por defecto.
2. **`tar -t`** (modo *table*/test): lista el contenido de un tarball **sin extraer nada** — como `ls` para archivos `.tar`. Inspeccionar con `tar -tf respaldo.tar` antes de decidir. `tar -x` extrae; `tar -c` crea.

## Dudas pendientes

- Ninguna por ahora. Próximo objetivo del plan: `find`, `grep` y pipes (`|`).

## Vocabulario nuevo (en inglés)

| Término | Significado |
|---|---|
| recursive | operación que se aplica a subdirectorios también (ej. `ls -R`, `-r`) |
| human-readable | formato de tamaño legible para personas (`ls -h`: KB/MB/GB) |
| append | añadir al final sin borrar (`>>`), a diferencia de `>` (sobrescribir) |