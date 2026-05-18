<div align="center">

<br>

# CALC∞

### Premium Scientific Calculator Platform

*Engineered with Apple-grade precision. Built for every screen.*

<br>

[![Live Demo](https://img.shields.io/badge/Live-Demo-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://arupdas0825.github.io/scientific-calculator/scientific-complex-calculator.html)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-f7df1e?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Math.js](https://img.shields.io/badge/Powered%20By-Math.js-FF9F0A?style=for-the-badge)](https://mathjs.org/)
[![Mobile First](https://img.shields.io/badge/Mobile-First-30D158?style=for-the-badge)](#)
[![License](https://img.shields.io/badge/License-MIT-0A84FF?style=for-the-badge)](LICENSE)

<br>

> A next-generation scientific calculator built with obsessive attention to detail —  
> pixel-perfect on mobile, powerful on desktop, always fast.

<br>

<img width="1918" height="971" alt="image" src="https://github.com/user-attachments/assets/faa88906-39f5-4e40-95e4-b81ec983725a" />

<br>

</div>

---

## What's New in v2.0

This is a complete ground-up rebuild. Not a patch. Not a refresh. Everything was redesigned from scratch with one goal: build the calculator that doesn't exist yet.

| Area | Before | After |
|---|---|---|
| Design system | Generic glassmorphism | Apple Calculator DNA — pure black, orange operators, depth layers |
| Mobile support | Basic responsive | `100dvh`, safe-area-insets, notch & home bar aware |
| Layout | Single view | Adaptive — bottom sheet on mobile, sidebar on desktop |
| Scientific mode | Always visible | Clean toggle — Standard / Scientific pills |
| Graph engine | Static render | Pan, scroll-to-zoom, pinch-to-zoom, multi-function, live coords |
| Solvers | None | Linear, Quadratic (complex roots), Right Triangle |
| Constants | None | 12 physical & mathematical constants — tap to insert |
| History | Basic list | Time-stamped, tap to recall, swipe sheet |
| Operators | Static | Active state highlight — exactly like native iOS |
| Angle mode | Fixed | DEG / RAD toggle with live calculation wrapping |
| Memory | None | MC · MR · M+ · M− with visual badge |
| 2ND key | None | Transforms sin↔sin⁻¹ · cos↔cos⁻¹ · ln↔eˣ dynamically |
| Typography | System font | JetBrains Mono + Figtree — intentionally chosen |
| Keyboard | None | Full keyboard input support |

---

## Live Demo

**👉 Open Calculator:** https://arupdas0825.github.io/scientific-calculator/scientific-complex-calculator.html

---

## Feature Breakdown

### Calculator Modes

**Standard Mode** — The everyday calculator. Clean. Minimal. Exactly what you need.

**Scientific Mode** — Expands to 5 columns with a full function row. Tap `2ND` to access inverse functions without cluttering the layout.

```
Standard:   AC  ±  %  ÷
            7   8  9  ×
            4   5  6  −
            1   2  3  +
            0      .  =

Scientific adds:
  2nd  sin  cos  tan  ln
  log  x²   xʸ   √   n!
  (    )    π    e    ⌫
```

### Mathematical Functions

```
Trigonometry      sin · cos · tan · asin · acos · atan
Hyperbolic        sinh · cosh · tanh
Logarithms        ln(x) · log₁₀(x) · log₂(x)
Powers & Roots    x² · x³ · xʸ · √x · ∛x
Factorial         n!
Exponential       eˣ · 10ˣ
Constants         π · e · φ · √2
Parentheses       Nested expression support
Percentage        % operator
Memory            MC · MR · M+ · M−
```

### DEG / RAD Toggle

All trigonometric functions automatically wrap their inputs and outputs based on the selected angle mode. Switch mid-session — results update correctly.

### 2ND Key System

One press transforms the scientific row:

| Normal | 2ND |
|---|---|
| sin | sin⁻¹ (asin) |
| cos | cos⁻¹ (acos) |
| tan | tan⁻¹ (atan) |
| ln | eˣ |
| log | 10ˣ |
| x² | x³ |

### Memory System

| Key | Action |
|---|---|
| MC | Clear memory |
| MR | Recall memory into expression |
| M+ | Add current display to memory |
| M− | Subtract current display from memory |

A `MEM` badge appears on the display whenever memory is loaded.

---

## Tools Workspace

Tap the graph or clock icon on mobile to open the bottom sheet. On desktop it renders inline as a sidebar automatically.

### Graph Plotter

- Plot multiple functions simultaneously with individual colors
- **Pan** by dragging (mouse or touch)
- **Zoom** with scroll wheel or pinch gesture on mobile
- **Live coordinates** — hover/touch shows real-time x · y values
- Configurable X range
- Color picker — Orange · Red · Green · Blue · Purple · Teal

```js
// Example functions you can plot
sin(x)
x^2 / 5
cos(x) * 2
tan(x)
sqrt(abs(x))
```

### Equation Solver

**Linear:** `ax + b = c` → solves for x

**Quadratic:** `ax² + bx + c = 0`
- Real roots: shows x₁ and x₂
- Double root: indicates repeated solution
- Complex roots: shows `a ± bi` form

**Right Triangle:** Given sides a and b → finds hypotenuse c, angle A, angle B

### Physical Constants

Tap any constant to insert its value directly into the calculator expression.

| Symbol | Constant |
|---|---|
| π | Pi — 3.14159265… |
| e | Euler's number — 2.71828… |
| φ | Golden ratio — 1.61803… |
| c | Speed of light — 299,792,458 m/s |
| h | Planck constant — 6.626×10⁻³⁴ J·s |
| G | Gravitational constant — 6.674×10⁻¹¹ |
| kB | Boltzmann constant — 1.380×10⁻²³ J/K |
| NA | Avogadro's number — 6.022×10²³ mol⁻¹ |
| e⁻ | Electron charge — 1.602×10⁻¹⁹ C |
| me | Electron mass — 9.109×10⁻³¹ kg |
| R | Gas constant — 8.314 J/mol·K |
| √2 | Square root of 2 — 1.41421… |

### Calculation History

- Stores up to 60 recent calculations
- Time-stamped (`30s ago`, `5m ago`, etc.)
- Tap any entry to recall the expression
- Clear all with one tap

---

## Mobile Experience

Built mobile-first. Every decision was made with a phone in hand.

```
✓  100dvh — correct height on iOS Safari including bottom bar
✓  env(safe-area-inset-*) — notch & home indicator aware
✓  user-scalable=no — no accidental zoom on double-tap
✓  apple-mobile-web-app-capable — installable as home screen app
✓  Touch ripple on every key press
✓  Swipe down to dismiss bottom sheet
✓  Pinch-to-zoom on graph canvas
✓  Touch pan on graph canvas
✓  Pointer events — no 300ms tap delay
✓  -webkit-tap-highlight-color removed
✓  Compact layout auto-adjusts for landscape
```

---

## Desktop Experience

On screens wider than 768px the layout switches automatically:

- Calculator on the left (fixed sidebar)
- Tools workspace on the right (persistent)
- No sheet required — everything visible at once
- Full keyboard input

```
Keyboard Shortcuts:
  0–9, .       → Number input
  + − * /      → Operators
  Enter or =   → Calculate
  Backspace    → Delete last character
  Escape       → Clear
```

---

## Design System

The visual language is built on a strict set of decisions — nothing arbitrary.

```
Background      Pure black #000000
Surface layers  #1C1C1E → #2C2C2E → #3A3A3C  (iOS system grays)
Number keys     #333333 — dark charcoal
Function keys   #A5A5A5 — light gray, black text
Operator keys   #FF9F0A — Apple orange
Active operator White background, orange text
Error state     #FF453A — system red
Success flash   Orange tint on result

Typography
  Display font   Figtree — geometric, modern, warm
  Mono font      JetBrains Mono — precise, readable at any size

Motion
  Spring easing  cubic-bezier(0.34, 1.56, 0.64, 1)
  Key press      scale(0.88) — physical, tactile
  Result flash   scale pop animation
  Sheet open     translateY spring — 400ms
  Toast slide    translateY + opacity — 200ms
```

---

## Tech Stack

| Technology | Role |
|---|---|
| HTML5 | Semantic structure, meta viewport, PWA meta |
| CSS3 | Design system, adaptive layout, animations |
| JavaScript ES6+ | State management, calculation engine, event handling |
| Math.js 11.11 | Expression parsing, scientific functions, complex numbers |
| Google Fonts | Figtree + JetBrains Mono |
| Canvas API | Real-time graph rendering with interaction |

Zero frameworks. Zero build tools. One file.

---

## Project Structure

```
scientific-calculator/
│
├── scientific-complex-calculator.html   ← entire app (single file)
└── README.md
```

The entire application — HTML, CSS, JavaScript — lives in one self-contained file. No dependencies to install, no build step, no server required.

---

## Run Locally

```bash
# Clone
git clone https://github.com/arupdas0825/scientific-calculator.git

# Enter directory
cd scientific-calculator

# Open directly in browser
open scientific-complex-calculator.html

# Or use Live Server in VS Code
```

---

## Supported Calculations

```
✓  Basic arithmetic           +  −  ×  ÷
✓  Scientific functions       sin · cos · tan · log · ln · √
✓  Inverse functions          asin · acos · atan
✓  Powers & exponents         x² · x³ · xʸ · eˣ · 10ˣ
✓  Roots                      √x · ∛x
✓  Factorials                 n!
✓  Parenthetical expressions  nested ( )
✓  Percentage                 %
✓  Memory operations          MC · MR · M+ · M−
✓  Constants                  π · e · φ · c · h · G · kB · NA
✓  Graph plotting             multi-function · pan · zoom
✓  Equation solving           linear · quadratic · triangle
✓  DEG / RAD modes            angle-aware trig
✓  Complex roots              quadratic with imaginary solutions
✓  Keyboard input             full hardware keyboard support
```

---

## Roadmap

- [ ] Unit converter (length, mass, temperature, currency)
- [ ] Matrix operations (2×2 and 3×3)
- [ ] Polar / Cartesian coordinate conversion
- [ ] Themes — Light mode, OLED ultra-dark, High contrast
- [ ] Expression history with search
- [ ] Programmer mode — HEX · BIN · OCT · AND · OR · XOR
- [ ] Statistics — mean, median, standard deviation
- [ ] PWA — offline support, install prompt
- [ ] Haptic feedback API (supported devices)

---

## Contributing

```bash
1. Fork the repository
2. Create your feature branch
   git checkout -b feature/your-feature-name
3. Commit your changes
   git commit -m "Add: your feature description"
4. Push to the branch
   git push origin feature/your-feature-name
5. Open a Pull Request
```

Please keep PRs focused. One feature per pull request.

---

## License

MIT License — free to use, modify, and distribute with attribution.

---

<div align="center">

## Author

**Arup Das**

[GitHub](https://github.com/arupdas0825)

<br>

---

*Built with precision, obsession, and zero compromise.*

**CALC∞ — Where computation meets craft.**

</div>
