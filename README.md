# BMI Calculator

> Calculate your Body Mass Index (BMI) using metric or imperial units and get simple tips for each category.

---

## Features

- **Dual unit systems** — Metric (kg, cm) and Imperial (lb, ft/in)
- **Bilingual** — Full Vietnamese 🇻🇳 and English 🇬🇧 support with Vietnamese-compatible font (Be Vietnam Pro)
- **Material Design 3** — Clean, accessible UI following Google's Material You design system
- **Theme support** — Light, Dark, and System-auto theme switching
- **Persistent preferences** — Language, unit system, and theme are saved to `localStorage`
- **BMI Gauge** — Visual indicator highlighting the active BMI category
- **Health Tips** — Contextual tips for each BMI category (Underweight / Normal / Overweight / Obese)
- **WHO Reference Table** — Full BMI classification table with the user's current category highlighted
- **Favicon** — Inline SVG favicon
- **No dependencies** — Pure HTML + CSS + Vanilla JS, no frameworks or CDN bundles required (only Google Fonts)

---

## BMI Categories (WHO)

| Category | BMI Range |
|---|---|
| Severe Thinness | < 16.0 |
| Moderate Thinness | 16.0 – 16.9 |
| Mild Thinness | 17.0 – 18.4 |
| **Normal weight** | **18.5 – 24.9** |
| Overweight | 25.0 – 29.9 |
| Obese Class I | 30.0 – 34.9 |
| Obese Class II | 35.0 – 39.9 |
| Obese Class III | ≥ 40.0 |

---

## Getting Started

No build step required. Just open `index.html` in any modern browser.

```bash
# Clone or download the project, then:
open index.html
# or serve locally:
npx serve .
```

---

## Project Structure

```
bmi-calculator/
├── index.html      # Main application (self-contained)
├── favicon.svg     # SVG favicon
└── README.md       # This file
```

---

## User Preferences (localStorage)

The following settings are remembered across sessions via `localStorage` under the key `bmi_prefs`:

| Key | Values | Default |
|---|---|---|
| `lang` | `vi` / `en` | `vi` |
| `unit` | `metric` / `imperial` | `metric` |
| `theme` | `light` / `dark` / `system` | `system` |

---

## Browser Support

Works in all modern browsers: Chrome, Firefox, Safari, Edge (last 2 versions).

---

## License

Free to use for personal and educational purposes.
