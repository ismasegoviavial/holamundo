# Implementation Plan — Hola Mundo Definitive Visual Redesign

Perform a complete visual overhaul of the **Hola Mundo** website to create an energetic, authentic, professional, and joyful brand identity for an **international online Spanish academy for kids & teens (ages 8–17)**.

---

## User Review Required

> [!IMPORTANT]
> - **Realistic Photography Focus**: Replaces all AI/3D renders and caricatures with authentic, natural lifestyle photography of real kids and teenagers (ages 8 to 17) actively engaged in online classes with laptops and headphones.
> - **Brand Palette**:
>   - **Navy Blue (`#0F172A` / `#1E3A8A`)**: Deep identity, trust, and headers.
>   - **Vibrant Sun Yellow (`#F59E0B` / `#FBBF24`)**: CTA buttons, badges, handwritten highlights, and energy.
>   - **Teal / Seafoam (`#0D9488` / `#E6FFFA`)**: Secondary accents and subtle backgrounds.
>   - **Clean White / Linen Cream (`#FFFFFF` / `#FAF9F6`)**: Background & generous white space.
> - **Custom Typography**:
>   - Headings: `Fredoka` & `Outfit` (Google Fonts CDN) — Friendly, rounded, modern, highly legible.
>   - Body: `Plus Jakarta Sans` — Clean, crisp, professional.
>   - Handwritten Accent: `Caveat` — For playful organic quotes (*"More than a class, it's an experience."*).
> - **New Visual Sections**:
>   - *Hero Section*: Asymmetric split with large realistic photo of a student with headphones on a laptop, yellow CTA, and adventure headline.
>   - *Our Approach ("Classes kids look forward to")*: Lifestyle photo composition, feature highlights, handwritten quote.
>   - *A Class at Hola Mundo ("This is what learning looks like")*: Step-by-step visual process (`01 Meet your group` → `02 Discover mission` → `03 Speak & play` → `04 Real conversation` → `05 Progress`).
>   - *Age Journeys*: Authentic age-specific photography for Explorers (8-10), Adventurers (11-13), and Teens (14-17).
> - **Retained Functionality & Email Setup**:
>   - All form submissions sent to **`educamaxcl@gmail.com`** via FormSubmit AJAX API.
>   - Anti-spam honeypot field (`_honeypot`).
>   - Bilingual `EN | ES` translator engine.
>   - 100% standalone, portable single-file `index.html`.

---

## Architecture & Layout Plan

```
hola-mundo-app/
└── index.html      # Self-contained file containing:
                    # - Full HTML5 Semantic Markup
                    # - Embedded CSS Design Tokens (Navy, Yellow, Teal, Cream)
                    # - Embedded Typography (Fredoka, Outfit, Plus Jakarta Sans, Caveat)
                    # - Unsplash/Pexels Authentic Photography URLs
                    # - Embedded JS App Core, i18n Dictionary & FormSubmit AJAX Handler
```

---

## Verification Plan

### Automated & Browser Verification
- **Double-Click Verification**: Open `index.html` directly in browser via `file://` scheme to ensure offline portability, zero console errors, and instant loading.
- **Photo Authenticity Audit**: Ensure all photos display real children and teenagers (ages 8 to 17) in natural light with zero AI/caricature artifacts.
- **Language Switch Test**: Test instant `EN | ES` translation across all new sections (Hero, Our Approach, A Class at Hola Mundo, Age Journeys, Faculty, FAQs, Modals).
- **Form Submission Test**: Verify FormSubmit AJAX post to `educamaxcl@gmail.com` with anti-spam honeypot and in-page success modal.
- **Mobile Responsive Check**: Verify drawer menu, sticky CTA bar, and editorial photo flow on mobile (375px) and desktop (1200px+).

---

## Next Steps
Upon user review, we will generate the updated single-file `index.html` and refresh the workspace artifact.
