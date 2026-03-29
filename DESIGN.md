# Design System Specification: High-Impact Cinematic Minimalist

## 1. Overview & Creative North Star: "The Digital Lens"
The Creative North Star for this design system is **The Digital Lens**. In an era of cluttered interfaces, this system acts as a sophisticated viewfinder, prioritizing the raw power of full-screen video content while providing a high-end, editorial UI layer that feels "projected" rather than "pasted."

This system breaks the "template" look by rejecting traditional boxed containers. Instead, it utilizes **intentional asymmetry** and **tonal depth**. UI elements should feel like floating glass panes, using extreme negative space (referencing our `20` and `24` spacing tokens) to allow the background cinematography to breathe. The goal is a "Quiet Luxury" aesthetic where the interface only commands attention when interacted with, maintaining a ghost-like presence otherwise.

---

## 2. Colors & Surface Philosophy
The palette is built on deep obsidian and cool slate tones to ensure legibility against diverse video backgrounds without "fighting" the footage.

### The "No-Line" Rule
Standard 1px solid borders are strictly prohibited for sectioning. Structural boundaries must be defined solely through background color shifts or subtle tonal transitions. For example:
- A `surface-container-low` (`#FFFFFF`) section should sit directly on a `surface` (`#FFFFFF`) background. The transition is the boundary.

---

## 5. Components

### Input Fields
* **Styling:** Transparent backgrounds with a `surface_variant` bottom-stroke only.
* **Focus State:** The bottom stroke transitions to `primary` (`#c4c7c9`) with a subtle `primary_dim` outer glow.

---

## 6. Do's and Don'ts

### Do:
* **DO** use `surface_container_lowest` for background overlays to ensure text remains readable over bright video spots (e.g., a sun flare).
* **DO** embrace asymmetry. Offset your Display text to the left and your action buttons to the right to create a dynamic "path" for the eye.
* **DO** use the `24` (`8.5rem`) spacing token for top and bottom page margins to maximize the cinematic impact of the video.

### Don't:
* **DON'T** use pure white (`#FFFFFF`) for text. Always use `on_surface` (`#dfe4ff`) or `primary` (`#c4c7c9`) to avoid "vibrating" against the video background.
* **DON'T** use `rounded-none`. Even the most minimal elements should have at least the `DEFAULT` (`0.25rem`) corner radius to feel premium and intentional.
* **DON'T** use drop shadows on text. If text is unreadable over video, increase the opacity of the underlying "Glass" surface layer instead.

---

## 7. Signature Interaction: The "Shimmer"
All primary CTAs and containers should feature a subtle "Shimmer" on hover—a translation of a linear gradient across the surface. This mimics the way light catches the edge of high-end watch crystals or architectural glass, reinforcing the premium nature of this design system.