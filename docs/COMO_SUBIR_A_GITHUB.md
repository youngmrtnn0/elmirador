# Cómo subir esto a GitHub (paso a paso)

Figma **no se conecta directamente a GitHub**. La forma correcta para este
trabajo es: exportar capturas de cada versión del prototipo + documentar los
cambios en este repo, y subirlo tú mismo. Sigue estos pasos:

## 0. Antes de empezar — Agregar a tus 2 compañeros como colaboradores
1. En la página del repo → **Settings** → **Collaborators** (menú izquierdo)
2. **Add people** → busca su usuario de GitHub de cada uno → **Add**
3. Ellos deben aceptar la invitación que les llega por correo/notificación

Así, cuando cada uno suba su parte, quedará registrado con SU propia
cuenta en el historial de commits — eso es lo que demuestra trabajo en
equipo real ante el profesor.

## 1. Crear el repositorio en GitHub
1. Entra a https://github.com → botón **New repository**
2. Nombre sugerido: `elmirador-subsistema-estructura`
3. Marca como **Public** (o Private + agrega al profesor como colaborador)
4. NO marques "Add README" (ya lo tienes en esta carpeta)
5. Clic en **Create repository**

## 2. Subir los archivos (dos formas)

### Opción A — Sin usar la terminal (más fácil)
1. En la página del repo recién creado, clic en **uploading an existing file**
2. Arrastra toda la carpeta `elmirador-repo` (README.md, CHANGELOG.md, /docs, /assets)
3. Escribe como mensaje de commit: `feat: estructura inicial del repositorio`
4. Clic en **Commit changes**

Para subir cada corrección por separado (recomendado, para que se vea el
historial real de versiones):
1. Edita o agrega archivos desde la pestaña **Add file > Upload files**
2. En el mensaje de commit, usa el prefijo correspondiente, ej:
   `fix: agrega badge de notificaciones y acciones en tabla de unidades`
3. Repite por cada corrección que vayan haciendo

### Opción B — Con Git instalado (si tienes terminal/Git instalado)
```bash
cd elmirador-repo
git init
git add .
git commit -m "feat: estructura inicial del repositorio y documentación v1.0.0"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/elmirador-subsistema-estructura.git
git push -u origin main
```

Luego, para cada nueva corrección:
```bash
git add .
git commit -m "fix: agrega badge de notificaciones en topnav"
git tag v1.1.0
git push origin main --tags
```

## 3. Cada integrante construye y sube su parte (hoy, con su propia cuenta)
Revisen `PROMPTS.md` para ver qué pantallas le tocan a cada uno.

1. Cada integrante construye sus pantallas en Figma con sus prompts
   asignados
2. Exporta sus capturas (clic derecho en el frame → **Copy/Export as PNG**,
   o `Ctrl+Shift+E` / `Cmd+Shift+E` para exportar varias a la vez)
3. Las sube a su carpeta correspondiente en `/assets`:
   - `assets/v1.0.0-login-residente` (Integrante 1)
   - `assets/v1.0.0-dashboard-ocupacion` (Integrante 2)
   - `assets/v1.0.0-comunidades-torres-unidades` (Integrante 3)
4. En GitHub: **Add file → Upload files**, sube sus imágenes a su carpeta
5. Mensaje de commit: usa el sugerido en `PROMPTS.md` para esa pantalla, ej:
   ```
   feat: agrega pantalla de login con accesos demo (RF1)
   ```
6. Repite por cada pantalla que le corresponda

## 4. Ronda final de correcciones (todos juntos)
1. Apliquen el prompt de correcciones (sección final de `PROMPTS.md`)
2. Exporten capturas nuevas a `assets/v1.1.0-correcciones`
3. Suban con los commits `fix:` sugeridos en `PROMPTS.md`

## 5. Qué mostrar en la presentación
- El historial de commits de GitHub (pestaña **Commits**) demuestra el
  control de cambios semántico exigido en el entregable, con los 3
  integrantes apareciendo como autores reales.
- El `CHANGELOG.md` resume en lenguaje natural cada corrección, ideal para
  explicar "los cambios en el prototipo" durante los 7 minutos de exposición.
- `PROMPTS.md` sirve como respaldo si el profesor pregunta cómo se construyó
  cada pantalla específicamente.
