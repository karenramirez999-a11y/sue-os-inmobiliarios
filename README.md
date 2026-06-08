# Sueños Inmobiliarios — Landing Page

Proyecto web estático listo para desplegar en Vercel.

---

## 📁 Estructura del proyecto

```
suenos-vercel/
├── index.html      ← Toda la landing page (CSS + JS incluidos)
├── vercel.json     ← Configuración de Vercel
└── README.md       ← Este archivo
```

---

## 🚀 Cómo desplegar en Vercel

### Opción A — Subir a GitHub y conectar con Vercel (recomendado)

**Paso 1: Crear repositorio en GitHub**
1. Ve a https://github.com y crea una cuenta si no tienes
2. Haz clic en **"New repository"**
3. Nombre: `suenos-inmobiliarios`
4. Ponlo en **Public** o **Private** (ambos funcionan)
5. Haz clic en **"Create repository"**

**Paso 2: Subir los archivos**

Opción sin instalar Git (más fácil):
1. En tu repositorio vacío, haz clic en **"uploading an existing file"**
2. Arrastra los 3 archivos: `index.html`, `vercel.json`, `README.md`
3. Haz clic en **"Commit changes"**

Opción con Git (terminal):
```bash
git init
git add .
git commit -m "Landing Sueños Inmobiliarios"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/suenos-inmobiliarios.git
git push -u origin main
```

**Paso 3: Desplegar en Vercel**
1. Ve a https://vercel.com y regístrate con tu cuenta de GitHub
2. Haz clic en **"Add New Project"**
3. Selecciona el repositorio `suenos-inmobiliarios`
4. Haz clic en **"Deploy"**
5. ¡Listo! En 1 minuto tendrás tu URL pública tipo:
   `https://suenos-inmobiliarios.vercel.app`

---

### Opción B — Arrastrar carpeta directo a Vercel (más rápido)

1. Ve a https://vercel.com/new
2. Arrastra la carpeta completa `suenos-vercel` al área de drop
3. Haz clic en **"Deploy"**
4. ¡Listo en 30 segundos!

---

## 🌐 Dominio personalizado (opcional)

Si tienes un dominio como `suenosinmobiliarios.co`:
1. En Vercel ve a tu proyecto → **Settings → Domains**
2. Agrega tu dominio
3. Sigue las instrucciones para apuntar el DNS

---

## ✏️ Cómo actualizar la página

1. Modifica el archivo `index.html`
2. Sube el archivo actualizado a GitHub
3. Vercel detecta el cambio y redespliega **automáticamente**

---

## 📞 Datos de contacto actuales en la página

- **WhatsApp:** +57 320 692 2370
- **Email:** s.inmobiliariosejecafetero@gmail.com
- **Ubicación:** Pereira, Risaralda, Colombia
