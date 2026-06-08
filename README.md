# Sueños Inmobiliarios — Con Supabase

Landing page con propiedades cargadas dinámicamente desde Supabase.

---

## 📁 Archivos

```
suenos-vercel/
├── index.html        ← Landing completa con integración Supabase
├── vercel.json       ← Config de Vercel
└── README.md         ← Este archivo

supabase_setup.sql    ← Script SQL para crear la tabla en Supabase
```

---

## ⚡ Setup paso a paso

### PASO 1 — Crear proyecto en Supabase

1. Ve a **https://supabase.com** y crea una cuenta gratis
2. Haz clic en **"New project"**
3. Ponle nombre: `suenos-inmobiliarios`
4. Elige región: **South America (São Paulo)**
5. Espera ~2 minutos a que termine

---

### PASO 2 — Crear la tabla con el SQL

1. En tu proyecto Supabase, ve a **SQL Editor** (menú izquierdo)
2. Haz clic en **"New query"**
3. Pega TODO el contenido del archivo `supabase_setup.sql`
4. Haz clic en **"Run"**
5. Verás las propiedades de ejemplo insertadas ✅

---

### PASO 3 — Obtener tus credenciales

1. En Supabase ve a **Settings → API**
2. Copia:
   - **Project URL** → algo como `https://trbamfvvpdmmdxpjiiqx.supabase.co`
   - **anon public key** → una clave larga que empieza con `us-east-1`

---

### PASO 4 — Configurar el index.html

Abre `index.html` y busca estas 2 líneas (están cerca del inicio del `<script>`):

```javascript
const SUPABASE_URL = 'https://trbamfvvpdmmdxpjiiqx.supabase.co';
const SUPABASE_ANON_KEY = 'us-east-1';
```

Reemplaza con tus valores reales:

```javascript
const SUPABASE_URL = 'https://trbamfvvpdmmdxpjiiqx.supabase.co';
const SUPABASE_ANON_KEY = 'us-east-1';
```

---

### PASO 5 — Desplegar en Vercel

**Opción A — Arrastrar carpeta (30 segundos):**
1. Ve a **https://vercel.com/new**
2. Arrastra la carpeta `suenos-vercel`
3. Deploy ✅

**Opción B — Con GitHub (recomendado):**
1. Crea repo en GitHub → sube los 3 archivos
2. Conecta en Vercel → Deploy
3. Cada actualización en GitHub = redeploy automático ✅

---

## 🏠 Agregar propiedades reales

En Supabase ve a **Table Editor → propiedades** y haz clic en **"Insert row"**:

| Campo | Ejemplo |
|-------|---------|
| titulo | Apartamento Pinares |
| precio | 380000000 |
| ciudad | Pereira |
| descripcion | Hermoso apto con vista panorámica... |
| imagen | https://tuurl.com/foto.jpg (opcional) |
| area | 85 |
| habitaciones | 3 |
| banos | 2 |
| tipo | Apartamento |
| estrato | Estrato 4 |
| parqueadero | 1 parqueadero |
| caracteristicas | ["🚗 Garaje","🏊 Piscina"] |
| activo | true |

---

## 🔄 Cómo funciona el flujo

```
Usuario abre la página
    ↓
JavaScript llama a Supabase API
    ↓
Supabase devuelve propiedades activas
    ↓
Se generan las tarjetas dinámicamente
    ↓ (si Supabase falla)
Se muestran 4 propiedades de ejemplo
```

---

## 📞 Contacto configurado

- WhatsApp: +57 320 692 2370
- Email: s.inmobiliariosejecafetero@gmail.com
