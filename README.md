# CADENCE — a reporting system that runs itself

A short, public overview of a system I designed and built end to end: it gathers a brand's numbers
from nine different platforms, reconciles the places where they disagree, writes the commentary,
runs its own quality checks, and publishes a finished performance report — work that previously took
an analyst most of a morning, every day.

**Live page:** `https://Saurabhpandey-1212.github.io/cadence-reporting-engine/`

The page is deliberately short. It's meant to be understood in about a minute by someone who clicked
a link on a résumé, with the technical detail tucked into one expandable section for readers who
want it.

---

## What's on the page

- What the system does, in plain language
- Four outcome numbers
- **An interactive demo** — press one button and watch a reporting cycle run step by step, ending in a
  finished sample report. It is a simulation: it runs entirely in the browser on generated sample
  data and makes no network calls of any kind.
- A five-stage "how it works" summary
- One collapsed section with technical detail

## The design rule behind it

> The AI layer is allowed to judge and explain, never to do the arithmetic. Every published figure is
> computed in code; the commentary is machine-checked against those figures before anything is
> allowed to publish.

## What is not published here

Source code, prompts, schemas, reconciliation rules, thresholds, adapter implementations, endpoints
and deployment details are proprietary and stay that way. No client data, real metrics or credentials
appear anywhere in this repository — every figure in the demo is generated in the browser, and the
four headline numbers are rounded measurements from the running system.

---

## Files

```
.
├── index.html    # the entire page — HTML, CSS and JavaScript in one self-contained file
├── LICENSE
├── README.md
└── .gitignore
```

`index.html` is the only file that matters. No build step, no dependencies, no CDN, no external
fonts — open it directly in a browser and it works.

## Deploying to GitHub Pages

1. Push this directory to a repository named `cadence-reporting-engine`.
2. **Settings → Pages → Source: Deploy from a branch**, branch `main`, folder `/ (root)`.
3. The page is live at the URL above within a minute or two.

Light theme by default with a dark toggle that persists, responsive from 320 px up, readable with
JavaScript disabled, and respects `prefers-reduced-motion`.

---

Designed and built by **Saurabh Pandey** · GreenHonchos · 2026
