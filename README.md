# Velvet Pour — Cocktail & Mocktail Bar

A visually rich, animation-driven single-page website for **Velvet Pour**, a cocktail and mocktail bar. Built with React and powered by GSAP scroll-driven animations for a cinematic browsing experience.

![React](https://img.shields.io/badge/React-19.1-61DAFB?logo=react&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-6.3-646CFF?logo=vite&logoColor=white)
![GSAP](https://img.shields.io/badge/GSAP-3.13-88CE02?logo=greensock&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-4.x-06B6D4?logo=tailwindcss&logoColor=white)

## Features

- **Scroll-pinned hero video** — Background video scrubs through its duration as you scroll, creating a cinematic intro
- **Character & line animations** — Hero titles split into characters and animate in with staggered reveals using GSAP SplitText
- **Parallax layers** — Decorative leaf elements move at different scroll speeds across multiple sections
- **Masked image reveal** — "The Art" section uses scroll-driven scaling and masking to dramatically unveil a cocktail image
- **Interactive cocktail carousel** — Tab-based menu slider with animated image and detail transitions
- **Responsive design** — Adapts layouts and animations for mobile and desktop via `react-responsive`
- **Noise texture overlay** — Subtle grain effect for a premium, editorial aesthetic

## Tech Stack

| Layer | Technology |
|---|---|
| Framework | React 19 |
| Build Tool | Vite 6 |
| Styling | Tailwind CSS 4 |
| Animations | GSAP 3.13 + ScrollTrigger + SplitText |
| React GSAP Integration | `@gsap/react` (`useGSAP` hook) |
| Responsive Utilities | `react-responsive` |

## Project Structure

```
├── constants/
│   └── index.js            # Navigation links, drink lists, cocktail data
├── public/
│   ├── images/             # Logos, leaves, drinks, about section imagery
│   ├── videos/             # Hero background video
│   └── fonts/              # Modern Negra custom typeface
└── src/
    ├── App.jsx             # Root layout, GSAP plugin registration
    ├── index.css           # Tailwind config, fonts, custom utilities
    ├── main.jsx            # React entry point
    └── components/
        ├── Navbar.jsx      # Fixed nav with scroll-aware background
        ├── Hero.jsx        # Animated hero + pinned video
        ├── Cocktails.jsx   # Drink lists with parallax leaves
        ├── About.jsx       # Story section with staggered image grid
        ├── Art.jsx         # Scroll-driven masked image reveal
        ├── Menu.jsx        # Interactive cocktail carousel
        └── Contact.jsx     # Footer with address, hours & socials
```

## Getting Started

### Prerequisites

- Node.js 18+
- npm or yarn

### Installation

```bash
git clone https://github.com/your-username/Mocktail-GSAP.git
cd Mocktail-GSAP
npm install
```

### Development

```bash
npm run dev
```

Open [http://localhost:5173](http://localhost:5173) in your browser.

### Production Build

```bash
npm run build
npm run preview
```

## Scripts

| Command | Description |
|---|---|
| `npm run dev` | Start Vite dev server with HMR |
| `npm run build` | Create optimized production build |
| `npm run preview` | Preview the production build locally |
| `npm run lint` | Run ESLint |

## Design System

- **Fonts** — Mona Sans, DM Serif Text, Modern Negra (custom)
- **Palette** — Black background, gold accent (`#e7d393`), soft white (`#efefef`)
- **Utilities** — Custom Tailwind classes for flex centering, text gradients, radial gradients, and masked images

## License

This project is for educational and demonstration purposes.
