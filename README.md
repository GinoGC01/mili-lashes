# 👁️ Lash Expert | Academy Landing Page

Landing page editorial de alto rendimiento desarrollada para **Milagro Ciancia**, lashista profesional y formadora especializada en extensiones de pestañas.  

El proyecto está enfocado en conversión premium mediante una experiencia visual cinematográfica y una arquitectura de Cero Hidratación para maximizar los Core Web Vitals.

---

## 🚀 Tech Stack

- **Framework:** Astro 5.x (SSG - Static Site Generation)  
- **Styling:** Tailwind CSS v4 (high-performance engine)  
- **Animations:** Native CSS + Intersection Observer API  
- **Icons:** Material Symbols (Google – thin variants)  
- **Assets:** Optimized SVG vector graphics  

---

## 🛠 Architecture & Technical Decisions

### 1️⃣ Cinematic Animation System

En lugar de librerías pesadas como Framer Motion, el proyecto implementa un sistema ligero de **"Reveal-on-Scroll"**:

- **GPU Layer Promotion**  
  Uso de `translate3d(0,0,0)` y `will-change` para promover elementos a la GPU y evitar jank en dispositivos móviles.

- **Staggered Entrance**  
  Retardos calculados (`animation-delay`) para guiar la atención del usuario con jerarquía visual.

---

### 2️⃣ High-End Editorial Design

- **Chrome Text Effect**  
  Gradientes lineales complejos + `background-clip: text` para simular acabados metálicos.

- **Optimized Glassmorphism**  
  Uso controlado de `backdrop-blur` con capas de opacidad para evitar sobrecarga del compositor.

- **Stacking Sections**  
  Uso estratégico de `z-index` y `position: sticky` para crear un efecto narrativo de secciones apiladas.

---

## 📂 Project Structure
```
├── public/
│ ├── images/ # SVGs optimizados y fotografías
│ └── fonts/ # Playfair Display & Poppins
├── src/
│ ├── components/ # Componentes atómicos de Astro
│ │ ├── Navbar.astro
│ │ ├── Hero.astro
│ │ ├── Programs.astro
│ │ └── ...
│ ├── layouts/ # Layout maestro (Head, SEO, scripts globales)
│ ├── pages/ # Rutas (index.astro)
│ └── styles/ # global.css con configuración Tailwind v4
└── astro.config.mjs
```

---
## 🔧 Development Setup

### Install dependencies

```bash
npm install
Start development server (HMR enabled)
npm run dev
Build for production
npm run build
