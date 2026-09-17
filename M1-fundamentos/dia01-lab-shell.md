---
tipo: lab
dia_plan: 01
fecha: 2026-09-17
modulo: M1-fundamentos
estado: ✅ hecho
tags: [shell, linux, comandos]
enlaces:
  - "diario/2026-09-17"
  - "M1-fundamentos/dia01-tema-shell"
---

# Día 1 · Lab — Fundamentos de Shell

> Práctica en terminal real · `pwd`, `ls`, `cd`, `cat`, `less`, `man`
> Evaluación: Fase 1 (conceptos) + Fase 2 (retos verificados) · 2026-09-17

## Situación

Campo de práctica: `labs/dia1-shell/practica/` con archivos `notas.txt`, `README.md`, `.secreto` (oculto), `numeros.txt` (100 líneas), `subdir/inner.txt`.

## Retos resueltos (verificados contra la máquina real)

| # | Reto | Comando | Verificado |
|---|---|---|---|
| 1 | Ver todos los archivos, incluido oculto, con tamaño | `ls -la` | ✅ |
| 2 | Navegar con ruta relativa y volver según convención | `cd practica/` → `cd ..` | ✅ |
| 3 | Leer archivo corto vs largo | `cat` corto · `less` largo | ✅ |
| 4 | Concatenar a archivo nuevo | `cat notas.txt README.md > combinado.txt` | ✅ (90 B, 6 líneas) |
| 5 | Inspeccionar un tarball sin extraer | `man tar` → `/list` → `tar -tf` | ✅ |

## Evidencia del reto 4 (la verifiqué con la terminal real, no por fe)

```
$ cat notas.txt README.md > combinado.txt
$ cat combinado.txt
hola mundo
segunda linea
fin
# README practica shell dia1

Este es un archivo de ejemplo.
$ wc -l combinado.txt      → 6
```

## Lo que se me escapó en la revisión (corregido)

1. **`ls -h`**: sin `-h` los tamaños son bytes brutos (`5000000`); con `-h` humanos (`4.8M`). Regla diaria: `ls -lh`.
2. **`tar -t`** (modo *table*/test): lista el contenido de un tarball sin extraer nada — el "`ls` de los `.tar`". Inspecciona con `tar -tf archivo.tar` antes de decidir.

_Nota: el concepto (por qué `less` sobre `cat`, redirección `>` vs `>>`) está en [[dia01-tema-shell]]._