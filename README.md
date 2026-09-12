## Tabla de contenido

| Archivo | Descripción |
|---|---|
| [01 · Modos y creación](docs/01-modos-y-creacion.md) | Modo normal, inserción y comando; cómo crear un archivo nuevo |
| [02 · Navegación](docs/02-navegacion.md) | Moverse dentro del archivo sin usar el mouse |
| [03 · Edición y deshacer](docs/03-edicion-y-deshacer.md) | Borrar, modificar y deshacer cambios |
| [04 · Copiar y pegar](docs/04-copiar-y-pegar.md) | Yank, delete y paste |
| [05 · Buscar y reemplazar](docs/05-buscar-y-reemplazar.md) | Búsquedas y sustituciones con `:s` |
| [06 · Insertar texto](docs/06-insertar-texto.md) | Distintas formas de entrar en modo inserción |
| [07 · Guardar y salir](docs/07-guardar-y-salir.md) | `:w`, `:q`, `:wq` y variantes |

---

## ¿Qué es `vi`?

> Vi, de visual, es un editor de texto nativo de cualquier sistema UNIX/Linux, este se diferencia de otros editores como Word - VS code - e inclusive nano. Esto se debe a que cuenta con modos de uso, estos son: 


> - Normal Mode: Es el modo predeterminado de arranque de Vi, en el cual las teclas escriben tal cual, sino que su función se asemeja más a una consola, teniendo la posibilidad de escribir comandos para diferentes usos tales como, borrar, copiar, deshacer, moverse, etc. 

> - Insertion Mode: En este modo, sí se inserta tal cual las letras en el documento, como se haría en cualquier otro editor. Para entrar a este modo, se presiona la tecla i y, para regresar al Normal Mode se presiona la tecla Esc.

> - Command Mode: Este tiene similitudes con el Normal Mode, pero está más enfocado a funciones como guardar (:w), salir (:q), etc, para acceder a este modo, se escriben los dos puntos :.

## `Cheat command table`

| Comando | ¿Qué hace? | Mi ejemplo |
|---|---|---|
| `i` | Entra en modo inserción antes del cursor | i |
| `Esc` | Vuelve al modo normal | Ecs |
| `:w` | Guarda el archivo | :w |
| `:q` | Sale del editor | :q |
| `:wq` | Guarda y sale | :wq |
| `dd` | Borra la línea actual | dd |
| `yy` | Copia (yank) la línea actual | yy |
| `p` | Pega después del cursor | p |
| `u` | Deshace el último cambio | u |
| `/palabra` | Busca "palabra" hacia adelante | /channel |
| `:%s/vieja/nueva/g` | Reemplaza todas las coincidencias en el archivo | :%s/configuration/configuracion/g |
| `gg` / `G` | Va al inicio / final del archivo | gg / G |


## ¿Cómo practicar tú mismo?

1. Clona este repositorio: g
   ```bash
   it clone https://github.com/NesperouDelmonico/Manual_editorVi_nvim_doomemacs.git
   ```
2. Abre el archivo de práctica con `vi`:
   ```bash
   vi ejercicios/mi-archivo-practica.txt
   ```
3. Repite los ejercicios descritos en cada archivo de `docs/`, en orden (del 01 al 07).

4. Guarda tus cambios con `:wq` y compara tu resultado con el archivo original usando:
   ```bash
   git diff ejercicios/mi-archivo-practica.txt
   ```
5. Si quieres reiniciar el ejercicio desde cero:
   ```bash
   git checkout -- ejercicios/mi-archivo-practica.txt



