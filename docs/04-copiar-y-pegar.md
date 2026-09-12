# 04 · Copiar y pegar

En `vi` no se llama "copiar", se llama **yank** (de ahí la tecla `y`). El concepto es el mismo: guardas texto en un "registro" temporal para pegarlo después.

## Copiar (yank)

| Comando | Efecto |
|---|---|
| `yy` | Copia la línea completa |
| `3yy` | Copia 3 líneas desde la actual |
| `yw` | Copia la palabra actual |
| `y$` | Copia desde el cursor hasta el final de la línea |

## Pegar (paste)

| Comando | Efecto |
|---|---|
| `p` | Pega **después** de la línea o el cursor actual |
| `P` | Pega **antes** de la línea o el cursor actual |

## Cortar (en realidad, "delete" también copia)

Algo que sorprende: en `vi`, cuando **borras** algo con `dd` o `x`, ese texto **también queda disponible para pegar** con `p`, igual que si lo hubieras copiado. Es decir, `dd` funciona como "cortar" (cut), no solo como "borrar".

## Ejemplo práctico

```bash
vi ejercicios/mi-archivo-practica.txt
```

1. Ubícate en una línea y presiona `yy` → la copias.
2. Muévete a otra línea con `j` o `k`.
3. Presiona `p` → la línea copiada aparece debajo de donde estás.
4. Ahora prueba con `dd` sobre otra línea, muévete, y presiona `p` → notarás que la línea "borrada" en realidad se movió (cortar y pegar).
