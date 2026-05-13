# Styling

Styling skills come in two flavors that work together: an **engine** that applies visual formatting to a SharePoint list, and a set of **style tokens** that define the colors, shapes, and typography the engine uses.

To style a list, install both:
1. The `list-styling` engine
2. One style token skill of your choice (e.g., `style-pastel`, `style-terminal`)

Then ask Copilot to style your list — the engine will read the tokens and apply them.

---

## Style Engine

The skill that does the work. Reads a style token file and applies the formatting to a SharePoint list or library.

| Folder | Skill | Description |
|---|---|---|
| [list-styling/](./list-styling/) | List Styling Engine | Transforms SharePoint lists and document libraries into fully art-directed views using column, view, and row formatting. Pairs with any of the style token skills below. |

---

## Style Tokens

Configuration skills that define a specific visual style. Each one provides the colors, shapes, typography, and component patterns that `list-styling` consumes. They don't do anything on their own — install one alongside the engine.

| Folder | Skill | Description |
|---|---|---|
| [style-bento/](./style-bento/) | Style: Bento | Bento-inspired horizontal compartment cards with warm earth tones, compact uppercase badges, and visible dividers. Triggers: *bento, warm style, earth tones, muted colors.* |
| [style-blueprint/](./style-blueprint/) | Style: Blueprint | Engineering-drawing aesthetic with a monochromatic blue palette, double-ring rubber-stamp badges, and an ultra-compact two-line spec-sheet card. Triggers: *blueprint, technical drawing, engineering, schematic, spec sheet.* |
| [style-figma-clean/](./style-figma-clean/) | Style: Figma Clean | Polished professional aesthetic with self-colored badge borders and thin precise progress bars. Triggers: *figma, clean style, polished, professional.* |
| [style-glassmorphism/](./style-glassmorphism/) | Style: Glassmorphism | Soft pill badges with no borders, thin bars, and an airy frosted-glass aesthetic. Triggers: *glassmorphism, frosted glass, glass look, soft modern.* |
| [style-high-contrast/](./style-high-contrast/) | Style: High Contrast | Maximum contrast ratios, larger fonts, thicker weights, and text indicators for WCAG accessibility compliance. Triggers: *high contrast, accessible, accessibility, WCAG, easy to read.* |
| [style-monochrome/](./style-monochrome/) | Style: Monochrome | A single slate-blue hue from light to dark replacing traffic-light colors — calm, corporate, tonal. Triggers: *monochrome, single color, one hue, corporate design system, all blue, tonal.* |
| [style-neobrutalism/](./style-neobrutalism/) | Style: Neobrutalism | Thick black borders, saturated colors, uppercase text, and hard offset shadows. Two-panel cards with red flip on overdue. Triggers: *neobrutalism, brutalist, bold borders, chunky style.* |
| [style-pastel/](./style-pastel/) | Style: Pastel | Soft candy colors with light tinted badge backgrounds and dark text — friendly and approachable. Triggers: *pastel, soft colors, candy, light badges, friendly style, approachable.* |
| [style-retro/](./style-retro/) | Style: Retro Memphis | Hot pink, electric blue, yellow, and teal with colored borders — bold, playful, nostalgic. Triggers: *retro, memphis, 80s, 90s, colorful, playful, bright colors.* |
| [style-terminal/](./style-terminal/) | Style: Terminal | Dark badges with neon green accents and matrix-style progress bars. Triggers: *terminal, hacker, dark mode, matrix, developer style, green on black.* |
