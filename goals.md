# Project Goals

## Mission

Provide comprehensive, accessible, and evidence-based fertility treatment information to help patients and couples make informed decisions during an emotionally challenging time.

## Completed

### v1.0.0 - Foundation
- [x] Astro static site setup with Netlify deployment
- [x] Core page structure (home, treatments, costs, resources)
- [x] Treatment pages for all major options (medication, IUI, IVF, third-party, preservation, surgical)
- [x] Cost comparison page with detailed breakdowns
- [x] Interactive Mermaid.js decision flowcharts
- [x] Mobile-responsive layout
- [x] Medical disclaimer

### v1.1.0 - Recurrent Loss
- [x] Recurrent pregnancy loss page with causes and treatments
- [x] RPL testing workup information
- [x] Treatment options for identified causes

### v1.2.0 - Causes & Statistics
- [x] Causes of infertility page
- [x] Male and female factor statistics
- [x] Citations to peer-reviewed sources (ASRM, ACOG, CDC, etc.)

### v1.3.0 - Miscarriage Statistics
- [x] Comprehensive miscarriage statistics
- [x] Age-based risk data
- [x] Risk reduction timeline during pregnancy
- [x] Global prevalence data with citations

### v1.4.0 - Visual Redesign
- [x] Modern gradient theme (#667eea to #764ba2)
- [x] Redesigned main pages (home, causes, treatments, costs, decision-guide, resources)
- [x] Redesigned all 7 treatment sub-pages
- [x] New component library:
  - [x] Gradient hero sections with breadcrumb navigation
  - [x] Card-based layouts with shadows
  - [x] Styled tables with gradient headers
  - [x] Callout boxes (info, warning, success)
  - [x] Stats cards with icons
  - [x] Process timelines
  - [x] Navigation footers between pages
- [x] Consistent visual language across all pages
- [x] Improved mobile responsiveness

## Future Ideas

### Content Expansion
- [ ] Male fertility dedicated page (expanded from current causes section)
- [ ] LGBTQ+ family building guide
- [ ] Single parent by choice resources
- [ ] International treatment options (medical tourism)
- [ ] Clinic comparison guide / what to look for
- [ ] Questions to ask your RE (reproductive endocrinologist)
- [ ] Glossary of fertility terms
- [ ] Timeline expectations for each treatment type

### Features
- [ ] Treatment cost calculator (interactive)
- [ ] Clinic finder integration
- [ ] Newsletter signup for updates
- [ ] Search functionality
- [ ] Print-friendly versions of pages
- [ ] PDF download option for treatment summaries
- [ ] Dark mode toggle

### Technical
- [ ] SEO optimization (meta tags, structured data)
- [ ] Performance audit and optimization
- [ ] Accessibility audit (WCAG compliance)
- [ ] Analytics integration
- [ ] Sitemap generation
- [ ] RSS feed for updates

### Community
- [ ] Success story submissions
- [ ] Community forum or discussion board
- [ ] Expert Q&A section
- [ ] Partner clinic/organization listings

## Design Principles

1. **Empathy First** - Users are often stressed, anxious, or grieving. Design should be calming and supportive.

2. **Evidence-Based** - All statistics and medical information cite peer-reviewed sources.

3. **Accessible** - Content should be understandable to non-medical audiences while remaining accurate.

4. **No Judgment** - Present all options neutrally without bias toward any particular path.

5. **Privacy Focused** - No tracking, no data collection, no ads.

## Content Guidelines

- Use plain language; explain medical terms when first introduced
- Provide cost ranges rather than exact figures (they vary significantly)
- Always cite sources for statistics
- Include both success rates AND limitations/risks
- Acknowledge emotional aspects alongside medical information
- Update statistics annually as new data becomes available

## Tech Decisions

| Decision | Rationale |
|----------|-----------|
| Astro | Fast static site, great DX, minimal JS |
| Vanilla CSS | No build complexity, easy to maintain |
| Mermaid.js | Interactive flowcharts without custom code |
| Netlify | Free hosting, easy deployment, fast CDN |
| No database | Static content, no user accounts needed |
| No analytics | Privacy focused, no tracking |

## Success Metrics

- Site loads in under 2 seconds
- All pages score 90+ on Lighthouse
- Content remains accurate and up-to-date
- Positive user feedback
- Zero accessibility violations
