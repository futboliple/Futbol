# Tabla del Fútbol ⚽

Archivos: `index.html` (la página) y `data.json` (jugadores y partidos).

## 1. Publicar en GitHub Pages
1. Crea una cuenta en github.com y un repositorio **público** nuevo (por ejemplo `futbol`).
2. Sube `index.html` y `data.json` (Add file → Upload files → Commit).
3. Ve a Settings → Pages → Source: "Deploy from a branch", rama `main`, carpeta `/ (root)` → Save.
4. En 1-2 minutos tu página estará en `https://TU-USUARIO.github.io/futbol/`. Ese es el enlace para el grupo: se ve sin iniciar sesión.

Si tu rama no se llama `main`, cambia `branch:"main"` al inicio del script en `index.html`.

## 2. Ser administrador (editar)
Solo pueden editar las personas con acceso de escritura al repositorio. Quien no lo tenga ve la tabla, pero no puede guardar nada, aunque intente.

**Dar acceso a otro admin:** Settings → Collaborators → Add people → su usuario de GitHub (debe aceptar la invitación).

**Cada admin crea su token (su "contraseña"):**
1. GitHub → foto de perfil → Settings → Developer settings → Personal access tokens → Fine-grained tokens → Generate new token.
2. Repository access: "Only select repositories" → elige `futbol`.
3. Permissions → Repository permissions → **Contents: Read and write**.
4. Genera y copia el token (empieza por `github_pat_`).

**Entrar en la página:** toca **🔐 Admin**, pega el token y entra. Aparece la pestaña ✏️ Editar y los botones de partidos. El token se guarda solo en ese navegador. **Cerrar sesión** lo borra. No compartas tu token con nadie.

## 3. Cómo se guarda
Cada vez que guardas, la página actualiza `data.json` en el repositorio. Los demás ven el cambio en 1-2 minutos. Si dos admins guardan a la vez, gana el último.

Para quitar a un admin: bórralo de Collaborators (su token deja de funcionar).
