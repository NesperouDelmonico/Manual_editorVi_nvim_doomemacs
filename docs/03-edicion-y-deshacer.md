# 03 · Edición y deshacer

## Borrar

| Comando | Efecto |
|---|---|
| `x` | Borra el carácter bajo el cursor |
| `dd` | Borra la línea completa |
| `dw` | Borra desde el cursor hasta el inicio de la siguiente palabra |
| `d$` | Borra desde el cursor hasta el final de la línea |
| `3dd` | Borra 3 líneas desde la actual (cualquier número funciona) |

## Modificar (cambiar) texto

| Comando | Efecto |
|---|---|
| `r` + letra | Reemplaza un solo carácter, sin entrar a modo inserción |
| `cw` | Borra la palabra actual y te deja en modo inserción para reescribirla |
| `cc` | Borra el contenido de la línea (conservándola) y entra en inserción |

## Deshacer y rehacer

| Comando | Efecto |
|---|---|
| `u` | Deshace el último cambio |
| `Ctrl + r` | Rehace (deshace el deshacer) |
| `U` | Deshace todos los cambios hechos en la última línea editada |

## Ejemplo práctico

```bash
vi ejercicios/mi-archivo-practica.txt
```

1. Ubícate sobre una línea y presiona `dd` → la línea desaparece.
2. Presiona `u` → la línea vuelve a aparecer (deshiciste el borrado).
3. Ubícate sobre una palabra y presiona `cw`, escribe una palabra nueva, `Esc` → reemplazaste la palabra sin borrar manualmente carácter por carácter.
4. Presiona `u` varias veces seguidas → puedes deshacer varios cambios en cadena, no solo el último.
