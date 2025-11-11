# 🚀 Instrucciones para Subir a GitHub

## Opción 1: Crear Repositorio desde GitHub (Recomendado)

### Paso 1: Crear repositorio en GitHub
1. Ve a [github.com](https://github.com) e inicia sesión
2. Click en el botón **"+"** → **"New repository"**
3. Configura:
   - **Repository name**: `analisis-entrenamientos-cx` (o el nombre que prefieras)
   - **Description**: `Análisis de implementación de material y reportes de entrenamiento`
   - **Visibility**: Private (recomendado para uso interno)
   - ⚠️ **NO** marques "Add a README file" (ya lo tenemos)
4. Click en **"Create repository"**

### Paso 2: Subir archivos desde terminal
```bash
# 1. Navegar a la carpeta donde están los archivos
cd /tmp

# 2. Inicializar git (si no existe)
git init

# 3. Agregar archivos
git add index.html README.md .gitignore

# 4. Hacer commit
git commit -m "Initial commit: Presentación análisis entrenamientos"

# 5. Conectar con GitHub (reemplaza <TU-USUARIO> y <TU-REPO>)
git remote add origin https://github.com/<TU-USUARIO>/<TU-REPO>.git

# 6. Subir archivos
git branch -M main
git push -u origin main
```

### Paso 3: Activar GitHub Pages (para verlo online)
1. En tu repositorio de GitHub, ve a **Settings**
2. Click en **Pages** (menú lateral izquierdo)
3. En **Source**, selecciona: **Deploy from a branch**
4. En **Branch**, selecciona: **main** → **/ (root)** → **Save**
5. Espera 1-2 minutos
6. Tu presentación estará en: `https://<TU-USUARIO>.github.io/<TU-REPO>/`

---

## Opción 2: Arrastrar y Soltar (Más Fácil)

### Paso 1: Crear repositorio en GitHub
(Igual que Opción 1, Paso 1)

### Paso 2: Subir archivos
1. En la página del repositorio recién creado, click en **"uploading an existing file"**
2. Arrastra estos 3 archivos:
   - `index.html`
   - `README.md`
   - `.gitignore`
3. Escribe en el commit: `Initial commit`
4. Click en **"Commit changes"**

### Paso 3: Activar GitHub Pages
(Igual que Opción 1, Paso 3)

---

## 📦 Archivos a Subir

Asegúrate de subir estos archivos:

```
✅ index.html              # La presentación
✅ README.md               # Documentación
✅ .gitignore             # Archivos a ignorar
```

---

## 🌐 Acceder a tu Presentación

Después de activar GitHub Pages:

**URL pública**: `https://<TU-USUARIO>.github.io/<TU-REPO>/`

Ejemplo: `https://alejandra-pinzon.github.io/analisis-entrenamientos-cx/`

---

## 🔒 Mantener Repositorio Privado

Si quieres que solo ciertas personas lo vean:

1. Ve a **Settings** del repositorio
2. En la sección **Danger Zone** → **Change repository visibility**
3. Selecciona **Private**
4. Para dar acceso: **Settings** → **Collaborators** → **Add people**

⚠️ **Nota**: GitHub Pages en repositorios privados requiere cuenta Pro/Enterprise

---

## 📝 Actualizar Presentación

Cada vez que hagas cambios:

```bash
# 1. Guardar cambios
git add .
git commit -m "Descripción de los cambios"
git push

# 2. Esperar 1-2 minutos para que GitHub Pages se actualice
```

---

## ❓ Problemas Comunes

### "Permission denied"
- Verifica que tu token de acceso esté configurado
- O usa: `git push https://<TOKEN>@github.com/<USUARIO>/<REPO>.git`

### "Remote already exists"
```bash
git remote remove origin
git remote add origin https://github.com/<TU-USUARIO>/<TU-REPO>.git
```

### Los archivos no se ven en GitHub Pages
- Verifica que el archivo se llame `index.html` (no `analisis_implementacion_material.html`)
- Espera 2-3 minutos después de activar Pages
- Revisa en Settings → Pages que esté "Active"

---

## ✅ Checklist Final

- [ ] Repositorio creado en GitHub
- [ ] 3 archivos subidos (index.html, README.md, .gitignore)
- [ ] GitHub Pages activado
- [ ] Presentación visible en la URL
- [ ] README se visualiza correctamente en la página principal

---

**¿Necesitas ayuda?** Revisa la [documentación de GitHub Pages](https://docs.github.com/pages)

