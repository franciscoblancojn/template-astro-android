# Mi App - Guía de Desarrollo

## Comandos

```bash
npm run dev          # Servidor de desarrollo (localhost:4321)
npm run build        # Build estático → dist/
npm run build:apk    # Build + APK → dist/template-astro-android.apk
npm run preview      # Preview del build
```

## Estructura

- `src/pages/index.astro` - SPA con 3 pantallas (Home, About, Settings)
- `src/scripts/app.js` - Entry point, navegación, orquestación
- `src/scripts/components/` - Componentes modulares
- `src/styles/main.css` - Estilos globales con temas light/dark
- `scripts/` - Build automation (post-build, build-apk)
- `android/` - Configuración Android (WebView wrapper)

## Arquitectura

- Framework: Astro (SSG) + vanilla JS
- Empaquetado: Android WebView
- Persistencia: localStorage
- Navegación: SPA manual con CSS animations
- Temas: Light/Dark con CSS custom properties
