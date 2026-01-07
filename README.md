# Function Practice Web App

This repository contains a simple front-end web app that generates 10 function-evaluation practice questions. Each question shows a function in LaTeX and provides a preset value of `x`. Students compute `f(x)` themselves and can click "Reveal" to see the correct value.

Functions include:

- Polynomials (degree up to 3)
- Rational functions
- Square roots
- Trigonometric (`sin`, `cos`)
- Logarithms (`ln`) and exponentials (`e^{...}`, `a^x`)

Math is rendered with KaTeX. A toggle lets you choose radians (default) for `sin`/`cos`.

## Quick Start

Open the app by loading `index.html` in your browser.

### Option 1: Open directly

Just double-click `index.html` or open it in your browser.

### Option 2: Serve locally (recommended)

Use any static server. For example with Python 3:

```bash
python3 -m http.server 8080
```

Then navigate to http://localhost:8080 in your browser and open `index.html`.

## How It Works

- Click "New Set of 10" to regenerate a fresh set of questions.
- For each question, evaluate the function at the provided value of `x`.
- Click "Reveal" to display the correct value for that `x`.

## Files

- `index.html`: The entire app (UI, logic, and styling). Uses KaTeX via CDN.

## Notes

- Trigonometric functions use radians by default; uncheck the toggle to treat `x` and linear arguments as degrees.
- Numeric outputs are formatted to a reasonable precision; very large/small results may display in scientific notation.
