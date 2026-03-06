# SEDEL Cotizador — App Móvil

Sistema de cotización de control de plagas para SEDEL.
Funciona como app instalable en iPhone y Android (PWA).

---

## Cómo publicar la app (sin experiencia técnica)

### Lo que necesitás instalar una sola vez en tu computadora

1. **Node.js** — descargá e instalá desde https://nodejs.org (elegí la versión "LTS")
2. **Git** — descargá e instalá desde https://git-scm.com

---

### PASO 1 — Subir el código a GitHub

1. Creá cuenta gratis en https://github.com
2. Hacé click en **"New repository"**
   - Nombre: `sedel-cotizador`
   - Dejalo en **Public**
   - Click en **"Create repository"**
3. Abrí una terminal (en Windows: buscá "PowerShell" o "CMD")
4. Escribí estos comandos uno por uno:

```
cd Desktop
cd sedel-app
git init
git add .
git commit -m "Primera versión"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/sedel-cotizador.git
git push -u origin main
```

> Reemplazá `TU_USUARIO` con tu nombre de usuario de GitHub

---

### PASO 2 — Publicar con Vercel (gratis)

1. Entrá a https://vercel.com
2. Hacé click en **"Sign up"** → elegí **"Continue with GitHub"**
3. Click en **"Add New Project"**
4. Seleccioná el repositorio `sedel-cotizador`
5. En la configuración dejá todo como está → click **"Deploy"**
6. En 2 minutos te da una URL como: `sedel-cotizador.vercel.app`

¡Ya está online!

---

### PASO 3 — Instalar en el celular

**En Android:**
1. Abrí Chrome en el celular
2. Entrá a tu URL de Vercel
3. Tocá los 3 puntitos (⋮) → **"Agregar a pantalla de inicio"**
4. Tocá **"Instalar"**

**En iPhone:**
1. Abrí Safari (tiene que ser Safari, no Chrome)
2. Entrá a tu URL de Vercel
3. Tocá el botón compartir (□ con flecha hacia arriba)
4. Tocá **"Agregar a pantalla de inicio"**
5. Tocá **"Agregar"**

La app aparece en la pantalla de inicio con el ícono de SEDEL,
se abre en pantalla completa y funciona sin internet.

---

### Actualizar la app cuando hacés cambios

Cuando modifiques el código, solo corré:
```
git add .
git commit -m "descripción del cambio"
git push
```
Vercel actualiza la app automáticamente en 1-2 minutos.

---

## Desarrollo local (para ver cambios en tiempo real)

```
npm install
npm run dev
```
Abrí http://localhost:5173 en el navegador.
