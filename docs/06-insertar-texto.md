# 06 · Insertar texto

Ya vimos `i`, `a`, `o` en el archivo de modos, pero aquí profundizamos en **cuándo conviene usar cada uno**, porque elegir el correcto te ahorra movimientos extra.

| Comando | ¿Dónde empieza a insertar? | Úsalo cuando... |
|---|---|---|
| `i` | Justo antes del cursor | Quieres agregar texto exactamente donde estás parado |
| `a` | Justo después del cursor | Quieres seguir escribiendo después del carácter actual |
| `I` | Al inicio de la línea (ignora espacios) | Quieres agregar algo al principio sin importar dónde esté el cursor |
| `A` | Al final de la línea | Quieres agregar algo al final sin importar dónde esté el cursor |
| `o` | Nueva línea debajo | Quieres escribir una línea nueva después de la actual |
| `O` | Nueva línea arriba | Quieres escribir una línea nueva antes de la actual |

## Salir de modo inserción

Siempre con `Esc`. No hay otra forma "segura" — usar el mouse o cerrar la terminal a medio escribir puede dejar el archivo en un estado raro.

## Ejemplo práctico

```bash
vi ejercicios/mi-archivo-practica.txt
```

1. Ubícate en cualquier línea y presiona `A` → el cursor salta al final de la línea, listo para escribir.
2. Escribe algo como ` <- agregado con A` y presiona `Esc`.
3. Presiona `o` → se abre una línea nueva debajo, ya en modo inserción.
4. Escribe una línea nueva y presiona `Esc` para volver a modo normal.
