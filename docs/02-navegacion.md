# 02 · Navegación

Toda la navegación ocurre en **modo normal**. Si estás en modo inserción, presiona `Esc` primero.

## Movimiento básico

| Comando | Movimiento |
|---|---|
| `h` | Izquierda |
| `j` | Abajo |
| `k` | Arriba |
| `l` | Derecha |

(Estas cuatro teclas existen porque en los teclados antiguos no siempre había flechas; hoy en día las flechas también funcionan, pero `hjkl` es más rápido al no mover la mano.)

## Movimiento por palabras y líneas

| Comando | Movimiento |
|---|---|
| `w` | Salta al inicio de la **siguiente** palabra |
| `b` | Salta al inicio de la palabra **anterior** |
| `e` | Salta al **final** de la palabra actual/siguiente |
| `0` | Va al inicio absoluto de la línea |
| `^` | Va al primer carácter no vacío de la línea |
| `$` | Va al final de la línea |

## Movimiento por el archivo completo

| Comando | Movimiento |
|---|---|
| `gg` | Va a la primera línea del archivo |
| `G` | Va a la última línea del archivo |
| `:n` | Va a la línea número `n` (ej: `:25`) |
| `Ctrl + f` | Avanza una pantalla completa |
| `Ctrl + b` | Retrocede una pantalla completa |

## Ejemplo práctico

Abre `ejercicios/mi-archivo-practica.txt` y prueba:

```bash
vi ejercicios/mi-archivo-practica.txt
```

1. `gg` → te posiciona en la primera línea.
2. `G` → saltas directo a la última línea.
3. `:10` → si el archivo tiene al menos 10 líneas, te lleva justo ahí.
4. `0` y luego `$` → te mueves del inicio al final de la línea actual.
