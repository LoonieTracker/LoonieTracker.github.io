# LoonieTracker Style Guide

## Overview
LoonieTracker.ca uses a minimalist, modern aesthetic inspired by financial tech design. The focus is on clarity, trust, and simplicity — helping Canadians learn about all-in-one ETFs (VEQT, XEQT, etc.) through clean typography, ample whitespace, and consistent use of teal as the brand accent.

---

## 1. Typography

**Primary Font:** [Inter](https://fonts.google.com/specimen/Inter)  
**Weights Used:** 400 (Regular), 600 (Semi-Bold), 700 (Bold)

### Font Usage
| Element | Font Size | Weight | Color | Example |
|----------|------------|--------|--------|----------|
| Page Title (h1) | 3rem–5rem (`text-5xl sm:text-6xl lg:text-7xl`) | 800 | `text-gray-900` | “Simple Investing. Max Returns.” |
| Section Title (h2) | 2rem–2.25rem (`text-4xl` or `text-3xl`) | 800 | `text-gray-900` | “Essential Canadian Investing Guides” |
| Subheading (h3) | 1.25rem (`text-xl`) | 600 | `text-gray-900` | “TFSA Explained” |
| Body Text | 1rem (`text-base`) | 400 | `text-gray-600` / `text-gray-500` | Paragraphs, descriptions |
| Small Text | 0.875rem (`text-sm`) | 400 | `text-gray-500` | Disclaimers, metadata |

---

## 2. Color Palette

### Brand Colors
| Name | Color | Usage |
|------|--------|--------|
| **Teal (Primary)** | `#0d9488` (Tailwind: `teal-600`) | Primary brand color for links, buttons, highlights |
| **Teal Light** | `#99f6e4` (Tailwind: `teal-100`) | Background for icons and highlights |
| **Teal Hover** | `#0f766e` (Tailwind: `teal-700`) | Hover and accent state |
| **Gray Dark** | `#1f2937` (Tailwind: `gray-800`) | Footer background |
| **Gray Medium** | `#6b7280` (Tailwind: `gray-500` / `gray-600`) | Body text |
| **Gray Light** | `#f9fafb` (Tailwind: `gray-50`) | Page background |
| **Accent Colors** | `blue-600`, `green-600`, `yellow-600` | Used in guide icons for visual differentiation |

---

## 3. Layout & Spacing

- **Max Width:** `max-w-7xl` (112rem)
- **Horizontal Padding:** `px-4 sm:px-6 lg:px-8`
- **Vertical Spacing:**
  - Section Padding Top/Bottom: `pt-12 pb-20`
  - Section Gaps: `mt-24`
  - Card Gaps: `gap-8`
- **Container Alignment:** Centered using `mx-auto`
- **White Space:** Prefer large spacing for readability and balance

---

## 4. Components

### Header
- Sticky top navigation (`sticky top-0 z-10`)
- White background (`bg-white`) with subtle shadow (`shadow-md`)
- Brand logo: bold teal text
- Nav links: `text-gray-600 hover:text-teal-600`

### Hero Section
- Center-aligned text with bold heading and subheading
- Two call-to-action buttons:
  - **Primary:** Teal button with shadow and hover scale animation  
    `bg-teal-600 hover:bg-teal-700 hover:scale-105`
  - **Secondary:** Outlined teal button  
    `border border-teal-600 text-teal-600 bg-white hover:bg-teal-50`

### Guide Cards
Reusable pattern for content blocks.

```html
<a class="block bg-white border border-gray-200 rounded-xl shadow-lg hover:shadow-2xl transform hover:-translate-y-1 p-6 transition">
  <div class="flex items-center justify-center h-16 w-16 rounded-full bg-teal-100 text-teal-600 mb-4">
    <!-- Icon -->
  </div>
  <h3 class="text-xl font-semibold text-gray-900 group-hover:text-teal-700">Title</h3>
  <p class="mt-2 text-gray-500 text-sm">Description</p>
</a>
```
**Rules:**

* Each card uses a distinct accent color (teal, blue, green, yellow)
* Include SVG icons for visual identity
* Use hover elevation and color change for interactivity

### Footer

* Background: `bg-gray-800`
* Text: `text-gray-300`, with teal highlights for links and headings
* Four-column responsive grid
* Divider line and copyright

---

## 5. Iconography

* **Source:** Heroicons (outline set)
* **Size:** `h-8 w-8` in cards, `h-5 w-5` in buttons
* **Style:** Rounded stroke, no fill (`fill="none"`, `stroke="currentColor"`)

---

## 6. Buttons

| Type          | Classes                                                                                                                              | Description   |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------------ | ------------- |
| **Primary**   | `px-8 py-4 text-base font-medium rounded-xl text-white bg-teal-600 hover:bg-teal-700 shadow-lg transition transform hover:scale-105` | Main CTA      |
| **Secondary** | `px-8 py-4 text-base font-medium rounded-xl border border-teal-600 text-teal-600 bg-white hover:bg-teal-50 transition`               | Secondary CTA |

---

## 7. Accessibility

* High contrast text-to-background ratios
* Semantic HTML (`<header>`, `<main>`, `<section>`, `<footer>`)
* SVG icons include `stroke` attributes and descriptive context
* Responsive layout from mobile to large screens

---

## 8. Responsive Design

| Breakpoint  | Tailwind Prefix | Notes                          |
| ----------- | --------------- | ------------------------------ |
| **Mobile**  | (none)          | Single-column layout           |
| **Tablet**  | `sm:` / `md:`   | Expands to 2-column grid       |
| **Desktop** | `lg:`           | Up to 4-column grid for guides |

---

## 9. Tone & Voice

LoonieTracker’s brand tone is:

* **Clear:** Avoid jargon and keep financial explanations simple.
* **Confident:** Present ETF investing as a calm, proven path.
* **Educational:** Use direct, helpful language.
* **Trustworthy:** Maintain a professional, transparent tone.

---

## 10. License & Attribution

* **Framework:** [Tailwind CSS](https://tailwindcss.com)
* **Icons:** [Heroicons](https://heroicons.com)
* **Font:** [Inter](https://fonts.google.com/specimen/Inter)
* **Copyright:** © 2026 LoonieTracker.ca. All rights reserved.

```
