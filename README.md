# Fertility Treatment Guide

A comprehensive static website providing information about fertility treatments, costs, and decision-making resources for patients and couples in the United States.

**Live Site:** [fertilitycentral.netlify.app](https://fertilitycentral.netlify.app)

## Overview

This site helps people navigating fertility treatments understand their options, compare costs, and make informed decisions. It includes:

- Detailed information on all major fertility treatment types
- Typical costs and price ranges
- Success rates with citations to medical literature
- Interactive decision flowcharts
- Insurance strategy guidance
- Support resources and financial assistance information

## Site Structure

```
/                              Home - Treatment overview and quick links
/causes/                       Causes of infertility with statistics
/treatments/                   Treatment options index
  /treatments/medication/      Fertility medications (Clomid, Letrozole, injectables)
  /treatments/iui/             Intrauterine insemination
  /treatments/ivf/             In vitro fertilization + PGT
  /treatments/third-party/     Donor eggs, sperm, embryos, surrogacy
  /treatments/preservation/    Egg and sperm freezing
  /treatments/surgical/        Surgical interventions
  /treatments/recurrent-loss/  Recurrent pregnancy loss
/costs/                        Cost comparison across all treatments
/decision-guide/               Interactive Mermaid.js flowcharts
/resources/                    Support organizations, financial assistance
```

## Design System

The site features a modern, accessible design with:

- **Color Palette:** Purple gradient theme (#667eea to #764ba2)
- **Typography:** System font stack for optimal performance
- **Components:**
  - Gradient hero sections with breadcrumb navigation
  - Card-based layouts with shadows and borders
  - Styled tables with gradient headers
  - Callout boxes (info, warning, success variants)
  - Stats cards with icons and metrics
  - Process timelines with numbered steps
  - Navigation footers linking between pages
- **Responsive:** Mobile-first design with breakpoints at 768px

## Tech Stack

- **Framework:** [Astro](https://astro.build/) v5.9
- **Flowcharts:** [Mermaid.js](https://mermaid.js.org/) via CDN
- **Styling:** Vanilla CSS with CSS custom properties
- **Deployment:** Netlify (Git integration with auto-deploy)
- **Repository:** GitHub

## Development

### Prerequisites

- Node.js 18+
- npm

### Setup

```bash
# Install dependencies
npm install

# Start development server
npm run dev
```

The dev server runs at `http://localhost:4321`

### Build

```bash
# Build for production
npm run build
```

Output is in the `dist/` directory.

### Preview Production Build

```bash
npm run preview
```

## Deployment

The site auto-deploys to Netlify on push to main branch.

### Manual Deployment

```bash
# Build and deploy
npm run build
netlify deploy --prod --dir=dist
```

## Versioning

The project uses semantic versioning with git tags.

```bash
# Bump patch version (1.0.0 -> 1.0.1)
npm version patch -m "v%s - Description"

# Bump minor version (1.0.0 -> 1.1.0)
npm version minor -m "v%s - Description"

# Bump major version (1.0.0 -> 2.0.0)
npm version major -m "v%s - Description"
```

Current version: **v1.4.0**

### Version History

| Version | Description |
|---------|-------------|
| v1.4.0  | Visual redesign of all pages with modern gradient theme |
| v1.3.0  | Add miscarriage and recurrent loss statistics |
| v1.2.0  | Add infertility causes and treatment statistics with citations |
| v1.1.0  | Add recurrent pregnancy loss content |
| v1.0.0  | Initial release |

## Project Structure

```
fertility-site/
├── src/
│   ├── layouts/
│   │   └── Layout.astro          # Main layout with header, footer, global styles
│   └── pages/
│       ├── index.astro           # Home page
│       ├── causes.astro          # Causes of infertility
│       ├── costs.astro           # Cost comparisons
│       ├── decision-guide.astro  # Mermaid flowcharts
│       ├── resources.astro       # Support resources
│       └── treatments/
│           ├── index.astro       # Treatments overview
│           ├── medication.astro
│           ├── iui.astro
│           ├── ivf.astro
│           ├── third-party.astro
│           ├── preservation.astro
│           ├── surgical.astro
│           └── recurrent-loss.astro
├── public/
│   └── favicon.svg
├── dist/                         # Build output
├── netlify.toml                  # Netlify configuration
├── astro.config.mjs
├── package.json
├── goals.md                      # Project goals and roadmap
└── README.md
```

## Content Sources

Statistics and success rates are cited from peer-reviewed sources:

- **CDC** - ART Success Rates
- **SART** - Society for Assisted Reproductive Technology
- **ASRM** - American Society for Reproductive Medicine
- **ACOG** - American College of Obstetricians and Gynecologists
- **NEJM** - New England Journal of Medicine
- **The Lancet** - Miscarriage statistics
- **PubMed/PMC** - Various studies

## Key Features

### Visual Design

Modern, calming aesthetic designed for users during a stressful time:
- Soft purple gradients convey professionalism and calm
- Card-based layouts make dense medical information digestible
- Clear visual hierarchy guides users through complex topics
- Consistent styling across all pages for seamless navigation

### Insurance Strategy Flowchart

Helps users with limited-cycle insurance coverage decide when to pay cash vs. use insurance benefits. Strategy: save covered cycles for expensive treatments (IVF, donor), pay out-of-pocket for cheaper options (meds, IUI).

### Decision Flowcharts

Interactive Mermaid.js diagrams covering:
- General treatment pathway
- Insurance strategy
- Treatment selection by diagnosis
- Age-based considerations
- IVF decision points
- Third-party reproduction paths
- Recurrent pregnancy loss pathway
- Fertility preservation timeline

### Cost Tables

Detailed breakdowns for each treatment type including:
- Procedure costs
- Medication costs
- Monitoring/labs
- Add-ons (PGT, ICSI, etc.)
- Total per-cycle estimates

## Commands

| Command             | Action                                      |
|---------------------|---------------------------------------------|
| `npm install`       | Install dependencies                        |
| `npm run dev`       | Start dev server at `localhost:4321`        |
| `npm run build`     | Build production site to `./dist/`          |
| `npm run preview`   | Preview build locally before deploying      |

## Disclaimer

This site provides general educational information only and is not a substitute for professional medical advice. Always consult with a qualified healthcare provider for personalized guidance.
