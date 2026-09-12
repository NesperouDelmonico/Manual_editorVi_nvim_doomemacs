# 05 · Buscar y reemplazar

## Búsqueda

| Comando | Efecto |
|---|---|
| `/palabra` + `Enter` | Busca "palabra" hacia **adelante** en el archivo |
| `?palabra` + `Enter` | Busca "palabra" hacia **atrás** |
| `n` | Repite la búsqueda en la misma dirección |
| `N` | Repite la búsqueda en dirección **contraria** |

## Reemplazo (sustitución)

El comando de sustitución sigue este patrón:

```
:[rango]s/patrón/reemplazo/[flags]
```

| Comando | Efecto |
|---|---|
| `:s/vieja/nueva/` | Reemplaza la **primera** coincidencia en la línea actual |
| `:s/vieja/nueva/g` | Reemplaza **todas** las coincidencias en la línea actual |
| `:%s/vieja/nueva/g` | Reemplaza **todas** las coincidencias en **todo el archivo** |
| `:%s/vieja/nueva/gc` | Igual que arriba, pero pide **confirmación** antes de cada cambio |

## Ejemplo práctico

```bash
vi ejercicios/mi-archivo-practica.txt
```

1. Escribe `/practica` + `Enter` → el cursor salta a la primera aparición de "practica".
2. Presiona `n` → salta a la siguiente coincidencia (si hay más de una).
3. Escribe `:%s/practica/ejercicio/g` + `Enter` → reemplaza **todas** las apariciones de "practica" por "ejercicio" en el archivo completo.
4. Si quieres revisar cada cambio antes de aplicarlo, usa `:%s/practica/ejercicio/gc` y responde `y` (sí) o `n` (no) para cada coincidencia.
