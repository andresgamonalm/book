# Brandformance Book — Andrés Gamonal

One-page profesional con la trayectoria, casos, recursos y datos de contacto de Andrés Gamonal.

## Estructura

```
.
├── index.html       ← El book completo (single file, sin dependencias)
├── README.md        ← Este archivo
└── .gitignore
```

Es un archivo HTML único con todo embebido (CSS, JS, SVG inline). Sin frameworks, sin build step, sin `node_modules`. Las únicas referencias externas son:

- Google Fonts (Roboto)
- Imágenes y PDFs alojados en `andresgamonal.com` y subdominios CDN (`cdn-gamonal`, `cdn-cv`, `cdn-liberty-andes`, `cdn-liberty-chile`, `cdn-bbva`, `cdn-santander`)
- Thumbnails y embeds de YouTube
- (Ningún tracker, ningún analytics)

## Cómo lo despliegas

Tres opciones, todas gratis:

### 1. GitHub Pages
1. Sube este repo a GitHub.
2. Repo → **Settings** → **Pages** → Source: `main` / root.
3. URL: `https://<usuario>.github.io/<repo>/` en 1–2 minutos.

### 2. Cloudflare Pages
1. Sube a GitHub.
2. En Cloudflare Dashboard → **Workers & Pages** → **Create application** → **Pages** → **Connect to Git**.
3. Selecciona el repo. Build settings: deja todo en blanco (es un sitio estático). Build output: `/`.
4. **Save and Deploy**. URL: `<proyecto>.pages.dev`.
5. (Opcional) Conecta tu dominio personalizado en Pages → **Custom domains**.

### 3. Netlify / Vercel
Conectas el repo y ya. Sin configuración. Detectan automáticamente que es estático.

## Cómo lo editas

Es un solo archivo. Abre `index.html` en tu editor favorito. Las secciones están comentadas con `<!-- NAV -->`, `<!-- HERO -->`, `<!-- ABOUT -->`, etc.

Cambios típicos:

- **Disponibilidad** (la píldora del hero "Disponible · Q3 2026") → buscar `Disponible · Q3 2026`
- **Texto del hero** → buscar "Bienvenido a mi"
- **Texto del Sobre mí** → buscar "Ejecutivo senior de marketing"
- **Marcas y casos** → buscar `id="c1"` … `id="c6"`
- **Certificaciones** (slide 2 del hero) → buscar "Certificaciones digitales 2026"
- **Email / WhatsApp / LinkedIn / CV** → buscar `mailto:`, `wa.me`, `linkedin.com/in/andresgamonal`, `cdn-cv.andresgamonal.com`

## Contenido incluido

- **Hero slider** con 2 slides: Bienvenida + Certificaciones
- **Stats**: 15+ años · 6 mercados · 5 compañías · Effie de Bronce
- **Disciplinas** en marquee: Estrategia, Performance digital, Publicidad masiva, Medios tradicionales, Research, IA, Producción audiovisual
- **Sobre mí**: bio profesional con Effie 2017
- **6 marcas**: Somos Radar (2026–), BMI Headquarters (2024–25), Liberty Andes (2020–24), Liberty Chile (2018–20), BBVA Chile (2014–18), Santander Chile (2012–14)
- **Recursos por caso**: 6 PDFs entregables, 4 PDFs infografías por país, 15 videos YouTube (con modal universal), 9 audios MP3, 1 PDF libro digital
- **Certificaciones** (Google, LinkedIn, HubSpot)
- **CV** descargable
- **Cierre** de búsqueda laboral con CTAs

## Notas técnicas

- Mobile-first responsive
- Sin difuminados / blur / glassmorphism
- Paleta Gamonal: navy `#040764`, blue `#1c73cb`, teal `#20b6b6`, yellow `#fce865`, charcoal `#3B3B3B`
- Tipografía: Roboto (300, 400, 500, 700, 900)
- Videos abren en modal con `youtube-nocookie.com` (menos restricciones de embed)
- Íconos de marca con fallback de color + iniciales si la imagen no carga

---

© Andrés Gamonal · Brandformance Lab
