# Portfolio Build Output (Modern Multi-Page, Light Mode)

## 1) Project Goal
Build a multi-page personal portfolio inspired by the listed references, with strong motion design, modern minimal UI, smooth interactions, and responsive behavior across devices.

---

## 2) Core Design Direction

### Visual Tone
- Creative, premium, minimal, futuristic.
- Light mode only.
- Pastel-leaning warm earthy palette from: https://coolors.co/palette/606c38-283618-fefae0-dda15e-bc6c25

### Color Tokens
- `--olive-700: #283618`
- `--olive-500: #606C38`
- `--cream-50: #FEFAE0`
- `--amber-400: #DDA15E`
- `--brown-600: #BC6C25`
- `--surface: #FFFDF4`
- `--text-primary: #1F2A16`
- `--text-secondary: #4A5537`
- `--border-soft: #E8E0C8`

### Typography
- Heading Font: **DM Sans**
- Body/UI Font: **Inter**
- Scale:
  - H1: 56/64
  - H2: 40/48
  - H3: 28/36
  - Body L: 18/30
  - Body: 16/26
  - Caption: 14/22

---

## 3) Recommended Tech Stack
- **Framework:** Next.js (App Router)
- **Language:** TypeScript
- **Styling:** Tailwind CSS + CSS variables
- **Animations:** Framer Motion + GSAP (for advanced timeline/scroll scenes)
- **3D/Visual Effects (optional):** React Three Fiber (constellation/rocket scenes)
- **Icons:** Lucide / Simple Icons
- **Forms:** React Hook Form + Zod
- **Deployment:** Vercel

---

## 4) Multi-Page Information Architecture
- `/` Home
- `/about` About + Certifications
- `/works` Works / Case Studies
- `/services` Services
- `/contact` Contact + FAQs
- `/404` Custom Not Found page with animation

Global elements:
- Animated loader (first visit / route transition)
- Sticky header with motion states
- Premium footer with glow/parallax/hover effects
- Shared transition system across pages

---

## 5) Motion & Interaction System

### Global Motion Rules
- Soft spring transitions (no harsh bounce).
- Section reveal on scroll (fade + translate + mask).
- Hover states on all interactive cards/buttons.
- Route transition overlay with subtle shape morph.

### Inspiration Mapping
- Portfolio inspiration (overall look + palette behavior):
  - https://www.wallofportfolios.in/portfolios/karthik-m/
  - https://www.wallofportfolios.in/portfolios/vishesh-gupta/
  - https://www.wallofportfolios.in/portfolios/rujul-s/
  - https://www.wallofportfolios.in/portfolios/hari-krishna/
- Technical skills + automation connection ideas:
  - https://cloudstudio.es/

### Specific Effects to Implement
1. **Home intro:** cinematic text reveal, layered parallax gradients, micro-particles.
2. **Motion cards:** tilt-on-hover, glow edge, depth shadow, icon morph.
3. **Automation connections:** animated node graph with flowing connection pulses.
4. **Tech stack scene:** rocket lift-off animation; stack logos as star-like points forming constellation paths.
5. **Footer special effect:** animated wave/noise background + orbiting accent particles + magnetic social icons.
6. **Loader:** brand monogram draw + progress line + fade-out.

---

## 6) Section-by-Section Content Blueprint

## Home
- Hero: name, title, short value statement, CTA pair (View Work / Contact).
- Animated intro statement with rotating keywords.
- Highlight stats strip (projects, certifications, years, clients/hackathons).
- Featured work teaser cards with motion.

## About (with Certifications)
- Professional summary narrative.
- Career timeline or milestones.
- Certifications grid/cards (issuer, certificate name, year, credential link).
- “How I work” principles section.

## Works
- Case study cards with category filters.
- Project details: problem, role, process, stack, outcome.
- Optional modal/page for each work item.
- Subtle scroll storytelling per case.

## Services
- Service cards (AI/ML solutions, web experiences, automation systems, consulting).
- For each: scope, deliverables, timeline band, CTA.
- Visual graphics + motion cards inspired from references.

## Contact (with FAQs)
- Contact form (name, email, project type, budget, message).
- Response expectation note.
- FAQ accordion with animated expand/collapse.
- Alternate contact channels + resume download button.

---

## 7) Asset Folder Structure (Single Organized Folder System)

Use one root assets directory:

```text
public/assets/
  brand/
    logo-primary.svg
    logo-mark.svg
    favicon.ico
  images/
    home/
    about/
    works/
    services/
    contact/
    shared/
  illustrations/
    rocket/
    constellation/
    automation/
  icons/
    tech/
    ui/
  animations/
    lottie/
    sprites/
  documents/
    resume.pdf
  seo/
    og-home.jpg
    og-default.jpg
```

Naming convention:
- `section-purpose-variant.ext`
- Example: `home-hero-bg-v1.webp`, `works-card-ai-vision-v2.webp`, `tech-logo-pytorch.svg`

---

## 8) README Content to Include

Your project README should contain:
1. Project overview + screenshots/GIFs
2. Live demo + repository links
3. Tech stack list
4. Installation and run steps
5. Environment variable setup
6. Folder architecture
7. Animation system notes (loader, route transitions, scroll reveals, constellation scene)
8. Custom 404 behavior and animation description
9. Accessibility and performance checklist
10. Content update guide (projects, certifications, FAQs, contact info)
11. Credits + references

Reference links section in README:
- https://www.wallofportfolios.in/portfolios/karthik-m/
- https://www.wallofportfolios.in/portfolios/vishesh-gupta/
- https://cloudstudio.es/
- https://www.wallofportfolios.in/portfolios/rujul-s/
- https://www.wallofportfolios.in/portfolios/hari-krishna/
- Palette: https://coolors.co/palette/606c38-283618-fefae0-dda15e-bc6c25

---

## 9) Responsive & Quality Requirements
- Mobile-first layout.
- Breakpoints: 320, 480, 768, 1024, 1280, 1536.
- All buttons/links keyboard accessible.
- `prefers-reduced-motion` support.
- Optimized media (WebP/AVIF), lazy loading, code splitting.
- Lighthouse target: 90+ performance/accessibility/best-practices.

---

## 10) Error States & Reliability
- Animated 404 page with guided return CTA.
- Form validation with inline messages.
- Fallback UI for animation-heavy sections.
- Include contact details and resume access in footer/contact for contingency.

---

## 11) Implementation Priority Roadmap
1. Design tokens + typography + layout grid
2. Shared components (header/footer/buttons/cards)
3. Home page hero + intro animation
4. About + certifications
5. Works + filters + case cards
6. Services motion cards
7. Contact + FAQs + validation
8. Tech stack rocket/constellation scene
9. Loader + route transitions + 404 animation
10. Performance pass + accessibility pass + content polish

---

## 12) Senior-Level Code Standards
- Strict TypeScript, reusable component architecture, clear naming.
- Isolated animation modules and constants.
- Reusable section schemas for maintainability.
- Error boundaries where needed.
- Consistent linting/formatting and documented component APIs.

