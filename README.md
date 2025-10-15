# 📘 Tipografía Modular — Violet Pulse

## 🎯 Propósito

Este módulo documenta la selección, uso y estructura de fuentes tipográficas empleadas en el sistema de diseño **Violet Pulse**. Está pensado para mantener consistencia visual, escalabilidad y legibilidad en interfaces modernas, contenido editorial y branding técnico.

---

## 🔠 Fuentes utilizadas

Las fuentes fueron seleccionadas por su popularidad en diseño web (2025), versatilidad y compatibilidad con interfaces técnicas y visuales.

| Variable SCSS        | Fuente         | Aplicación / Uso                         | Estilo clave                           |
|----------------------|----------------|------------------------------------------|----------------------------------------|
| `$font-title`        | Montserrat     | Titulares, branding, botones grandes     | Sans-serif geométrica, fuerte, elegante|
| `$font-subtitle`     | Inter          | Subtítulos, navegación, UI               | Sans-serif moderna, versátil           |
| `$font-content`      | Merriweather   | Contenido editorial, párrafos largos     | Serif legible, elegante, técnica       |
| `$font-ui`           | Manrope        | Dashboards, formularios, componentes UI  | Sans-serif técnica, minimalista        |
| `$font-base`         | Roboto         | Texto general, compatibilidad móvil      | Sans-serif neutra, confiable           |

---

## 📦 Instalación

### Opción 1: Google Fonts (en línea)

```html
<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@700&family=Inter:wght@400;600&family=Merriweather&family=Manrope:wght@400;600&family=Roboto:wght@400;700&display=swap" rel="stylesheet" />
```

## ✅ Alternativa: Usar fuentes de Google Fonts sin conexión

1. Descarga la fuente
Puedes descargar las fuentes desde:

🔗 https://fonts.google.com

    Busca cada fuente (por ejemplo, Montserrat, Inter, Merriweather, etc.), selecciona los pesos que necesitas (como 400, 600, 700), y haz clic en "Download family".

2. Organiza tu proyecto

    Crea una carpeta en tu proyecto, por ejemplo:

```
    /assets/fonts/
  └── montserrat/
  └── inter/
  └── merriweather/
```

3. Declara las fuentes en tu CSS o SCSS

```
@font-face {
  font-family: 'Montserrat';
  src: url('/assets/fonts/montserrat/Montserrat-Bold.woff2') format('woff2');
  font-weight: 700;
  font-style: normal;
  font-display: swap;
}

@font-face {
  font-family: 'Inter';
  src: url('/assets/fonts/inter/Inter-Regular.woff2') format('woff2');
  font-weight: 400;
  font-style: normal;
  font-display: swap;
}

@font-face {
  font-family: 'Merriweather';
  src: url('/assets/fonts/merriweather/Merriweather-Regular.woff2') format('woff2');
  font-weight: 400;
  font-style: normal;
  font-display: swap;
}

```


4. Usa las fuentes como siempre


```
body {
  font-family: 'Merriweather', serif;
}

h1 {
  font-family: 'Montserrat', sans-serif;
}

h2, h3 {
  font-family: 'Inter', sans-serif;
}


```
### 📋 Recomendaciones

- Usa clamp() para tamaños fluidos:

```
font-size: clamp(1rem, 2vw + 0.5rem, 2rem);

```
- Aplica font-display: swap para mejorar rendimiento
- Mantén jerarquía visual con una escala modular (1.125 o 1.25)