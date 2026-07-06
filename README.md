# SVG Path Image Hover Effect

An interactive image gallery where SVG paths animate on hover, revealing titles with a smooth stroke-draw effect. Built with GSAP, Lenis smooth scrolling, and Vite.

**Author:** AJ  
**By:** [anassjid](https://github.com/ajxdevx)

## Preview

Hover over any card to watch the SVG paths draw in and the title slide up word by word.

## Features

- Animated SVG path stroke on hover (dash offset + stroke width)
- SplitText word reveal for card titles
- Smooth scrolling with Lenis
- Responsive grid layout
- Per-card custom stroke colors

## Tech Stack

- [Vite](https://vitejs.dev/)
- [GSAP](https://gsap.com/) + SplitText
- [Lenis](https://lenis.darkroom.engineering/)

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or later recommended)

### Installation

```bash
npm install
```

### Development

```bash
npm run dev
```

Open the URL shown in the terminal (usually `http://localhost:5173`).

### Build

```bash
npm run build
npm run preview
```

## Project Structure

```
├── index.html      # Page markup and SVG paths
├── styles.css      # Layout and card styling
├── script.js       # GSAP hover animations and Lenis setup
├── public/         # Static assets (images)
└── package.json
```

## How It Works

1. Each card contains two overlapping SVG strokes and an image.
2. On `mouseenter`, GSAP animates `strokeDashoffset` from the path length to `0`, creating a draw effect, while stroke width expands.
3. Card titles are split into words with SplitText and slide up with a staggered animation.
4. On `mouseleave`, the animation reverses.

## License

ISC
