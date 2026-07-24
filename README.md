# Citation Matrix — Deduplicador & Explorador

Herramienta interactiva para limpiar la *citation matrix* de un umbrella review:
deduplica los estudios primarios que aparecen escritos de forma distinta en cada
revisión sistemática, etiqueta outcomes (VO2 · capacidad funcional · calidad de vida)
por revisión, y permite combinar el trabajo de dos personas.

Es un único archivo HTML autónomo: no necesita servidor ni base de datos.
Todo el avance se guarda/carga en archivos `.json` desde el propio navegador.

---

## Cómo publicarla en GitHub Pages (una sola vez)

1. Entra a https://github.com y crea un repositorio nuevo (botón **New**).
   - Nombre sugerido: `citation-matrix` · visibilidad **Public**.
2. En el repo vacío, pulsa **Add file → Upload files** y sube estos dos archivos:
   - `index.html`
   - `README.md`
   Confirma con **Commit changes**.
3. Ve a **Settings → Pages** (menú lateral).
   - En *Build and deployment* → *Source*: **Deploy from a branch**.
   - *Branch*: **main** · carpeta **/ (root)** → **Save**.
4. Espera ~1 minuto. GitHub te mostrará la URL pública, del tipo:
   `https://TU-USUARIO.github.io/citation-matrix/`

Ese link ya lo puedes compartir con tu equipo.

---

## Cómo actualizarla cuando queramos

1. En el repo, abre `index.html` y pulsa el lápiz ✏️ (**Edit**), o usa
   **Add file → Upload files** para reemplazarlo por una versión nueva.
2. **Commit changes**. En ~1 minuto la URL ya sirve la versión actualizada
   (puede requerir refrescar con Ctrl/Cmd + Shift + R).

> El link no cambia nunca; solo se actualiza el contenido. Por eso sirve como
> "versión oficial" del proyecto.

---

## Flujo de trabajo colaborativo (dos personas)

Publicar en un link **facilita el acceso**, pero NO es edición simultánea en vivo:
los datos viven en el navegador de cada persona. El avance se une por archivos.

1. Cada quien abre la URL y trabaja su parte (repártanse por revisión: p. ej. R1–R16 y R17–R33).
2. Cada quien pulsa **💾 Guardar sesión** → obtiene su `.json`.
3. Una persona carga su archivo (**📂 Cargar sesión**) y luego pulsa
   **🔗 Combinar sesión** eligiendo el `.json` de la otra.
4. Se **suman** ambos trabajos (etiquetas, fusiones y quitados) sin sobrescribir nada.
5. Guardar de nuevo → ese `.json` combinado es el respaldo maestro.

Para el manuscrito, la pestaña **Exportar** genera la matriz limpia en CSV/Excel.
