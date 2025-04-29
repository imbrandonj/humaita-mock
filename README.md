# humaita-mock

## Project Summary  
Front-end optimization and SEO refinement of the static website for Gracie Humaita Kansas City. The following changes were made to improve performance, structure, and discoverability.

---

## Performance Baseline (Original Site)

A Lighthouse audit on the original site failed to complete due to severe violations of modern web standards:

| Category       | Status     | Notes                                                      |
|----------------|------------|------------------------------------------------------------|
| Performance    | ❌ Failed   | Browser tab crashed. Metrics like LCP, FCP, CLS could not be calculated. |
| Accessibility  | ❌ Failed   | ARIA roles, landmark elements, labels, and keyboard navigation all missing or broken. |
| Best Practices | ❌ Failed   | Uses deprecated APIs, lacks HTTPS, violates CSP and HSTS recommendations. |
| SEO            | ❌ Failed   | Missing `<title>`, `<meta description>`, alt text, canonical tag, and hreflang. |

Captured: **Apr 29, 2025, 12:40 PM CDT**  
Lighthouse Version: **12.4.0**  
Environment: **Desktop** with **Chromium 135.0.0.0**

> **Lighthouse Metric Summary:**
> - **Performance:**
>   - **LCP – Largest Contentful Paint:** How long it takes the main content to load.
>   - **FCP – First Contentful Paint:** When something first appears; shows the site is alive.
>   - **CLS – Cumulative Layout Shift:** Measures layout jumping as content loads; a poor UX signal.
>   - **TBT – Total Blocking Time:** How long the browser is unresponsive due to heavy script execution.
>   - If these fail to calculate, it means the site did not load properly or crashed during audit.
>
> - **Accessibility:**
>   - Measures whether the site is usable by people with disabilities, including screen readers and keyboard navigation.
>   - Includes presence of alt text, correct label associations, logical tab order, and ARIA roles.
>   - i.e., an ARIA role defines the purpose of the HTML element for screen reading technology
>   - If this fails, the site may be inaccessible or unusable for assistive technologies.
>
> - **Best Practices:**
>   - Assesses modern coding standards and site security.
>   - Includes HTTPS usage, no deprecated APIs, secure headers, and safe script behavior.
>   - Failures suggest technical debt and security or compatibility risks.
>
> - **SEO:**
>   - Evaluates if the site is optimized to be found and indexed by search engines.
>   - Includes `<title>`, meta description, canonical URL, structured data, and alt text.
>   - A failed score here results in poor search engine visibility.

---

## Optimization & Asset Management

- **Logo Format**  
  Replaced `cropped-Gracie-Production.png` with `logo.webp` for modern image compression.  
  _Why: WebP is a newer format that reduces file size without sacrificing quality, improving load times._

- **Favicon Update**  
  Converted tab icon from PNG to `.ico` format for cross-browser compatibility.  
  _Why: `.ico` is the standard favicon format supported across all browsers and platforms._

- **Hero Banner**  
  Converted hero image to WebP format, reducing size from **21,389KB → 276KB** (~99% reduction).  
  _Why: A smaller file drastically reduces load time, especially on mobile connections._

- **Content Images**  
  All content images converted to WebP format with device-based size selection.  
  Example: Helio PNG reduced from **250KB → 30KB**.  
  _Why: Reduces bandwidth usage and improves page speed across devices._

---

## SEO & Semantic Improvements

- **Title Tag**  
  Added `<title>` tag with value `"Gracie Humaita Kansas City"`.  
  _Why: Clear, concise titles improve search ranking and avoid keyword penalties. Without it, browsers may fall back to using the `<h1>` as the tab label._

- **Meta Description**  
  Added: `"Gracie Humaita Kansas City offers competitive Brazilian Jiu Jitsu, self defense, and training for adults and kids."`  
  _Why: Helps Google understand what the site is about and display a clean search snippet._

- **Keyword Strategy Suggestions**  
  Include context-specific keywords like: `Academy`, `School`, `Gym`.  
  Add alt text to index.html image of kids BJJ class.  
  _Why: Relevant keywords and alt tags increase visibility in search and improve accessibility._

---

## Content & Layout Refinements

- **Text Cleanup**  
  Corrected grammar issues, eliminated extra spaces, refined phrasing.  
  _Example: “Women’s Brazilian Jiu Jitsu” section on index.html_  
  _Why: Clean, professional writing improves credibility and user experience._

- **Image Alignment**  
  Centered misaligned images and relocated them for logical flow and visual balance.  
  _Why: Visual consistency improves readability and aesthetic appeal._

- **Footer Overhaul**  
  - Changed copyright:
    ```
    "2025 Gracie Humaita Kansas City. All rights reserved."
    ```
  - Centered `Contact` and `Navigation` sections.  
  - Resized font and upgraded headers (`Contact`, `Navigation`) to `<h4>` elements.  
  _Why: Clear structure improves legibility and helps users navigate the site more easily._

---

