# 01 · Modos y creación de archivos

## Los tres modos de `vi`

| Modo | ¿Para qué sirve? | ¿Cómo entro? |
|---|---|---|
| **Normal** | Moverte, borrar, copiar, ejecutar comandos | Es el modo inicial / `Esc` desde cualquier otro modo |
| **Inserción** | Escribir texto nuevo | `i`, `a`, `o`, `I`, `A`, `O` (ver tabla abajo) |
| **Comando (línea)** | Guardar, salir, buscar/reemplazar en todo el archivo | `:` desde modo normal |

Regla de oro: **si no sabes en qué modo estás, presiona `Esc`**. Siempre te devuelve a modo normal sin riesgo de romper nada.

## Formas de entrar a modo inserción

| Comando | Efecto |
|---|---|
| `i` | Inserta **antes** del cursor |
| `a` | Inserta **después** del cursor (append) |
| `I` | Inserta al **inicio de la línea** |
| `A` | Inserta al **final de la línea** |
| `o` | Abre una **línea nueva debajo** y entra en inserción |
| `O` | Abre una **línea nueva arriba** y entra en inserción |

## Crear un archivo nuevo

```bash
vi notas.txt
```

Si `notas.txt` no existe, `vi` lo crea en memoria (no en disco todavía). No se guarda en disco hasta que uses `:w`.

### Ejemplo completo

```bash
vi saludo.txt
```

1. Presiona `i` para entrar a modo inserción.
2. Escribe: `Hola, este es mi primer archivo con vi`
3. Presiona `Esc` para volver a modo normal.
4. Escribe `:wq` y presiona `Enter` para guardar y salir.

```bash
cat saludo.txt
# Hola, este es mi primer archivo con vi
```
