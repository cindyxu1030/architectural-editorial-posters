---
name: architectural-editorial-posters
description: Create, adapt, or critique architecture-led editorial posters that combine photographic or rendered buildings with oversized typography, technical linework, translucent interface panels, curved spatial motifs, and a restrained accent palette. Use when the user asks for a poster, campaign key visual, event graphic, cover, social asset, or format variants inspired by futuristic architectural editorial design, especially when the aspect ratio may be portrait, square, landscape, ultrawide, or a custom size.
---

# Architectural editorial posters

Create a designed poster, not an architecture photo with decoration. Treat the building as the layout system: align type, panels, paths, and diagrams to its edges, openings, curves, depth, and perspective.

Read [poster-grammar.md](references/poster-grammar.md) before designing. Read [ratio-playbook.md](references/ratio-playbook.md) whenever the user requests a custom ratio, multiple formats, or a ratio change.

## Gather the brief

Collect or infer:

- exact canvas size or aspect ratio
- final-use context and likely viewing size
- exact text, language, and hierarchy
- subject, place, event, or campaign theme
- brand kit, logo, palette, and font constraints
- supplied images and each image's role: edit target, content source, or style reference
- preferred energy: technical, dreamlike, ecological, nocturnal, warm, or austere
- required export format and destination

Ask only when missing information would materially change the design. Otherwise make a clear assumption and proceed. If copy is long, propose a shorter hierarchy before shrinking everything.

## Protect identity and source boundaries

- Use reference posters to learn a visual grammar, not to copy a single composition.
- Do not reproduce source logos, creator marks, watermarks, disclaimers, slogans, or decorative pseudo-copy.
- Do not invent a client logo or substitute typed text for a supplied logo.
- When a brand kit conflicts with the references, keep the architectural composition logic and follow the brand kit for color, typography, logo, and claims.
- For Sonilo, use the current Sonilo brand guide. Keep its dark ground, indigo triad, Suisse family, and claim gates. Do not import the references' mixed serif/script typography or unrelated neon colors into Sonilo work.

## Build the composition

### 1. Find the architectural carrier

Choose one dominant structural feature that can carry the visual idea:

- stacked balconies or floors
- a sweeping ramp or facade curve
- a corner, clock, portal, or cylindrical bay
- a deep street canyon or atrium
- a glass volume that can behave like a transparent data panel

Use one carrier as the main gesture. Secondary motifs may support it but must not compete with it.

### 2. Choose one poster concept

Write a one-sentence concept that connects content to structure. Examples:

- "The facade becomes a vertical timeline."
- "A curved aquarium ramp carries the title through the building."
- "A glass bay behaves like a transparent analytical window."

Reject concepts that only name a mood. The concept must explain what the architecture does.

### 3. Establish hierarchy

Before sizing type from references, isolate the artwork bounds. If a reference is a phone screenshot, video-player capture, mockup, or framed presentation, exclude the app chrome, black bars, device frame, and surrounding UI. Measure type against the visible artwork, not the screenshot canvas.

Use four levels at most:

1. one dominant title or wordmark
2. one secondary phrase, subtitle, or script accent
3. a small information cluster
4. microtype, labels, or numeric texture

Only levels 1 to 3 need to be fully readable at normal viewing size. Microtype must still be intentional, but it cannot carry required information.

### 4. Compose the image layer

Use a real photo, user-supplied image, licensed media, or generated architectural image. Preserve useful negative space and a strong depth path.

When generating the image layer, use the built-in image generation tool by default. Ask it for the architecture and atmosphere without final typography, logos, watermarks, UI, charts, or random signs. Specify the target ratio and where clean space is needed.

### 5. Add deterministic typography and graphics

Build final text, borders, connector lines, panels, labels, and logos in a deterministic layout tool such as HTML/CSS, SVG, canvas, Canva, or the project's native design system. Do not rely on a generative image model for exact final text when another layout path is available.

Make overlays respond to the building:

- let a title sit behind and in front of architectural layers
- wrap a line or short phrase along a real curve
- anchor panel corners to facade joints
- let one accent path travel across depth
- rotate type only when it follows a strong structural edge

Keep linework sparse enough that the building remains legible.

## Adapt to any aspect ratio

Recompose. Never stretch a finished poster.

1. Calculate `R = width / height` and select the ratio family in [ratio-playbook.md](references/ratio-playbook.md).
2. Preserve the concept, hierarchy, palette, and architectural carrier.
3. Re-select the crop or regenerate the scene for the new frame.
4. Move modules into the new reading path. Do not preserve their old coordinates.
5. Keep all required content inside the safe zone.
6. Reduce decorative modules before reducing title legibility.

For a multi-format set, design the hardest ratio first. This is usually the narrowest portrait or widest landscape. Then derive the easier formats from the same concept.

## Produce and iterate

Create one strong direction first unless the user asks for alternatives. When alternatives are useful, vary the concept or carrier, not just the color.

For each direction, state:

- concept sentence
- aspect ratio and dimensions
- architectural carrier
- title treatment
- accent palette
- image-generation prompt for the image layer, if used
- final export path

Inspect the rendered poster at full size and thumbnail size. Make one targeted revision at a time.

## Quality gate

Do not deliver until all checks pass:

- exact aspect ratio and requested dimensions
- title readable at thumbnail size
- headline scale and placement are measured against the artwork bounds, not screenshot or mockup chrome
- required copy matches the brief character for character
- no generated gibberish, duplicate letters, fake logos, or watermark residue
- one dominant visual gesture, not several unrelated effects
- required title behaves as part of the architecture through scale, alignment, cropping, occlusion, curvature, or reflection; it does not read as a standalone card pasted over the image
- overlay geometry follows architectural structure or perspective
- adequate contrast behind required text
- safe margins survive platform cropping
- no copied source branding or near-duplicate source composition
- brand colors, fonts, logo use, and claims are correct when a brand kit applies
- export opens correctly and the final path is reported

If a final is generated as one raster image and contains text errors, do not call it finished. Rebuild the text layer deterministically or regenerate with less embedded text.
