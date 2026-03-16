# ⛅ SkyCast — Dashboard del Clima

Dashboard del clima construido con **Astro**, que muestra el clima actual y el pronóstico de 7 días para cualquier ciudad del mundo.

## 🛠 Herramientas usadas

- [Astro](https://astro.build/) — framework principal para la página estática
- [Open-Meteo API](https://open-meteo.com/) — datos meteorológicos (gratuita, sin API key)
- [Open-Meteo Geocoding API](https://open-meteo.com/en/docs/geocoding-api) — conversión de nombre de ciudad a coordenadas
- CSS personalizado con variables CSS (sin frameworks externos)
- JavaScript vanilla para fetch y manipulación del DOM
- Google Fonts: Syne + DM Mono

## ✨ Funcionalidades

- 🔍 Búsqueda de cualquier ciudad del mundo
- 🌡️ Temperatura actual, sensación térmica, humedad, viento y precipitación
- 📅 Pronóstico para los próximos 7 días
- 🌙 Dark mode con toggle y persistencia en `localStorage`
- 📱 Diseño responsive (mobile, tablet y desktop)
- ⚡ Componente reutilizable `WeatherCard`

## 🚀 Instrucciones para ejecutarlo

### Requisitos

- [Node.js](https://nodejs.org/) versión 18 o superior
- npm (viene incluido con Node.js)

### Pasos

```bash
# 1. Clonar el repositorio
git clone https://github.com/tu-usuario/weather-dashboard.git
cd weather-dashboard

# 2. Instalar dependencias
npm install

# 3. Correr en modo desarrollo
npm run dev
```

La página estará disponible en `http://localhost:4321`

### Build para producción

```bash
npm run build
npm run preview
```

## 📁 Estructura del proyecto

```
weather-dashboard/
├── src/
│   ├── layouts/
│   │   └── Layout.astro       # Layout principal con HTML base y estilos globales
│   ├── components/
│   │   └── WeatherCard.astro  # Componente reutilizable para las métricas
│   └── pages/
│       └── index.astro        # Página principal (única)
├── public/                    # Archivos estáticos
├── astro.config.mjs
├── package.json
└── README.md
```

## 🌐 Deploy

El proyecto puede deployarse fácilmente en [Vercel](https://vercel.com) o [Netlify](https://netlify.com) conectando el repositorio de GitHub.
