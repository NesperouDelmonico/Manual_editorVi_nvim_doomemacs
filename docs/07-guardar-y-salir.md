# 07 · Guardar y salir

Todos estos comandos se escriben en **modo comando**: primero `Esc` (para asegurarte de estar en modo normal) y luego `:`.

## Comandos principales

| Comando | Efecto |
|---|---|
| `:w` | Guarda (write) sin salir |
| `:q` | Sale, pero **solo si no hay cambios sin guardar** |
| `:wq` | Guarda y sale |
| `ZZ` | Atajo equivalente a `:wq` (sin necesidad de `Enter`) |
| `:q!` | Sale **sin guardar**, descartando todos los cambios |
| `:w nombre.txt` | Guarda una copia con otro nombre, sin afectar el archivo original |

## ¿Por qué `vi` a veces "no me deja salir"?

Si intentas `:q` y tienes cambios sin guardar, `vi` te lo va a impedir a propósito, mostrando un mensaje de error. Esto es una protección para que no pierdas trabajo por accidente. Tienes dos opciones:

- `:wq` → si quieres guardar los cambios y salir.
- `:q!` → si quieres **descartar** los cambios y salir de todas formas.

## Ejemplo práctico

```bash
vi ejercicios/mi-archivo-practica.txt
```

1. Haz un cambio cualquiera (entra con `i`, escribe algo, `Esc`).
2. Escribe `:q` + `Enter` → verás un error porque hay cambios sin guardar.
3. Escribe `:wq` + `Enter` → esta vez sí guarda y cierra.
4. Vuelve a abrir el archivo (`vi ejercicios/mi-archivo-practica.txt`) para confirmar que el cambio quedó guardado.
