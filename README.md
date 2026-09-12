# 📘 Manual de `vi` — Sobreviviendo al editor que todo sysadmin debe dominar

> Una guía práctica y personal sobre el editor `vi`, hecha a partir de mis propios ejercicios de laboratorio.

![Made with Markdown](https://img.shields.io/badge/Made%20with-Markdown-1f425f.svg)
![Status](https://img.shields.io/badge/status-en%20progreso-yellow)
![Tema](https://img.shields.io/badge/tema-editor%20vi-blue)
![Licencia](https://img.shields.io/badge/licencia-MIT-green)

---

## 📑 Tabla de contenido

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

## 🤔 ¿Qué es `vi`?

> ⚠️ **Pendiente de personalizar.** Esta sección debe estar escrita con tus propias palabras (2-3 párrafos), basada en lo que realmente entendiste durante la práctica — no copiada de ninguna guía. Te dejo aquí solo una guía de qué puntos podrías cubrir, no el texto final:
>
> - Párrafo 1: qué es `vi`, por qué existe, en qué contexto lo usaste (SSH, servidor sin entorno gráfico, etc.)
> - Párrafo 2: cómo se diferencia de un editor "normal" (los modos, por qué al principio se siente raro)
> - Párrafo 3: tu opinión / experiencia personal aprendiéndolo — qué se te dificultó, qué comando te salvó la vida

*(Borra este bloque de advertencia cuando escribas tu versión.)*

---

## 🧾 Cheat sheet — comandos esenciales

> ⚠️ Completa la columna "Mi ejemplo" con un caso real que tú hayas probado en `ejercicios/mi-archivo-practica.txt`.

| Comando | ¿Qué hace? | Mi ejemplo |
|---|---|---|
| `i` | Entra en modo inserción antes del cursor | *(pendiente)* |
| `Esc` | Vuelve al modo normal | *(pendiente)* |
| `:w` | Guarda el archivo | *(pendiente)* |
| `:q` | Sale del editor | *(pendiente)* |
| `:wq` | Guarda y sale | *(pendiente)* |
| `dd` | Borra la línea actual | *(pendiente)* |
| `yy` | Copia (yank) la línea actual | *(pendiente)* |
| `p` | Pega después del cursor | *(pendiente)* |
| `u` | Deshace el último cambio | *(pendiente)* |
| `/palabra` | Busca "palabra" hacia adelante | *(pendiente)* |
| `:%s/vieja/nueva/g` | Reemplaza todas las coincidencias en el archivo | *(pendiente)* |
| `gg` / `G` | Va al inicio / final del archivo | *(pendiente)* |

---

## 🧪 Cómo practicar tú mismo

1. Clona este repositorio:
   ```bash
   git clone https://github.com/<tu-usuario>/manual-vi-editor.git
   cd manual-vi-editor
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
   ```

---

## 🙏 Créditos

- Basado en la guía de laboratorio original proporcionada en el curso.
- Docente: *(nombre del docente)*
- Documentación y ejercicios adaptados por: *(tu nombre)*

---

## 📄 Licencia

Este proyecto se distribuye bajo la licencia especificada en [LICENSE](LICENSE) (opcional).
