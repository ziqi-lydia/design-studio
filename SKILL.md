---
name: design-studio
description: Professional design studio for non-designers. Creates social media graphics, dashboards, web pages, and slides with Apple-level aesthetics. Guides users through design decisions using intuitive metaphors instead of jargon.
---

# Design Studio — Professional Design for Non-Designers

## Purpose
Create professional-quality visual designs — social media graphics, dashboards, web pages, presentations, and marketing materials — for users who are not designers. Uses intuitive metaphors and plain language instead of design jargon.

## Core Philosophy
- **Apple-level aesthetics** as the baseline, not the ceiling
- **Intuitive metaphors** > design jargon (say "breathing room" not "whitespace")
- **Opinionated defaults** — don't ask users to choose fonts, pick for them
- **Show, don't ask** — generate the design first, iterate from there

---

## Design Principles

### 1. Visual Hierarchy
Every design has exactly ONE focal point. Everything else supports it.
- **Primary**: The thing you want people to see first (headline, hero image, CTA)
- **Secondary**: Supporting information (subheadline, description)
- **Tertiary**: Details (footer, metadata, fine print)

### 2. Typography Rules
- **Maximum 2 fonts** per design (1 heading + 1 body)
- **Font pairing**: Contrast in style (sans-serif heading + serif body, or vice versa)
- **Size hierarchy**: Heading should be 2-3x body text size
- **Line height**: 1.4-1.6x font size for body text
- **Letter spacing**: Slightly increased for all-caps text (+2-5%)

### 3. Color System
- **Maximum 3 colors** + black/white
  - Primary: Brand color or dominant accent
  - Secondary: Complementary or analogous
  - Accent: Used sparingly for CTAs and highlights
- **60-30-10 rule**: 60% dominant, 30% secondary, 10% accent
- **Contrast**: Text must pass WCAG AA contrast ratio (4.5:1 minimum)

### 4. Spacing & Layout
- **Consistent spacing** using a base unit (8px grid system)
- **Generous margins** — when in doubt, add more space
- **Alignment**: Everything aligns to something. Random placement = amateur
- **Golden ratio** for layout proportions when applicable

### 5. Image Guidelines
- **High quality only** — no pixelated, stretched, or watermarked images
- **Consistent style** — all images in one design should match in style (photo vs illustration vs icon)
- **Meaningful images** — every image should serve a purpose, not just fill space

---

## Output Formats

### Social Media Graphics
**LinkedIn Post Image**: 1200 x 627px
**LinkedIn Carousel**: 1080 x 1080px per slide
**Instagram Post**: 1080 x 1080px
**Instagram Story**: 1080 x 1920px
**Twitter/X Post**: 1200 x 675px

### Presentations
**Standard**: 1920 x 1080px (16:9)
**Vertical**: 1080 x 1920px (9:16)

### Web Pages
**Desktop**: 1440px wide, responsive down to 320px
**Generated as**: Single-file HTML with inline CSS

### Dashboard / Data Viz
**Generated as**: HTML with inline CSS and minimal JS for interactivity

---

## Design Templates

### Template 1: Bold Statement
Best for: LinkedIn posts, social media quotes, announcements
- Large centered text (hero statement)
- Subtle background gradient or solid color
- Brand logo or icon in corner
- Minimal — text IS the design

### Template 2: Split Layout
Best for: Before/after, comparison, two-sided arguments
- Vertical or horizontal split
- Contrasting colors on each side
- Balanced text on both halves
- Clear visual separation

### Template 3: Card Grid
Best for: Feature highlights, tool comparisons, listicles
- 2x2 or 3x2 grid of cards
- Icon + title + short description per card
- Consistent card styling
- Subtle shadows or borders

### Template 4: Hero + Body
Best for: Blog headers, landing pages, presentations
- Large hero image or illustration at top
- Headline overlaid or below
- Body text with clear hierarchy
- CTA button or next action

### Template 5: Data Dashboard
Best for: Metrics, KPIs, analytics reports
- Key metric cards at top (big numbers)
- Charts/graphs in the body
- Trend indicators (up/down arrows)
- Time period selector

### Template 6: Timeline / Process
Best for: Roadmaps, step-by-step guides, workflows
- Horizontal or vertical timeline
- Numbered steps with icons
- Progress indicators
- Brief descriptions per step

---

## Color Palettes (Pre-built)

### Professional / Corporate
- Primary: #1a1a2e (Dark Navy)
- Secondary: #16213e (Deep Blue)
- Accent: #0f3460 (Royal Blue)
- Highlight: #e94560 (Coral Red)

### Modern / Clean
- Primary: #2d3436 (Charcoal)
- Secondary: #636e72 (Slate)
- Accent: #0984e3 (Electric Blue)
- Highlight: #00cec9 (Teal)

### Warm / Friendly
- Primary: #2d3436 (Charcoal)
- Secondary: #fdcb6e (Warm Yellow)
- Accent: #e17055 (Coral)
- Highlight: #00b894 (Mint)

### Minimal / Elegant
- Primary: #2c3e50 (Dark Slate)
- Secondary: #ecf0f1 (Light Gray)
- Accent: #3498db (Calm Blue)
- Background: #ffffff (White)

### Dark Mode
- Primary: #1e1e2e (Dark Background)
- Secondary: #313244 (Card Background)
- Accent: #89b4fa (Soft Blue)
- Text: #cdd6f4 (Light Text)

---

## Implementation

### For HTML-based designs (web pages, dashboards)
Generate single-file HTML with:
- All CSS inline or in a `<style>` block
- Google Fonts loaded via CDN
- Responsive breakpoints
- No external dependencies

### For Image-based designs (social media graphics)
Use the `generateImage()` API with detailed prompts that specify:
- Exact layout and composition
- Color hex codes
- Typography hierarchy
- Element positioning

### For Presentations
Use the `pptx` skill for PowerPoint generation, applying design principles above.

---

## Quality Gates

Before delivering ANY design, verify:

### Layer 1: Technical
- [ ] Correct dimensions for target platform
- [ ] Text is readable at actual display size
- [ ] Colors pass contrast requirements
- [ ] No pixelated or stretched elements

### Layer 2: Composition
- [ ] Clear visual hierarchy (one focal point)
- [ ] Consistent spacing and alignment
- [ ] Maximum 2 fonts used
- [ ] Maximum 3 colors + black/white

### Layer 3: Content
- [ ] No spelling or grammar errors
- [ ] Text is concise (social media: <15 words per text block)
- [ ] Brand consistency (if brand guidelines exist)
- [ ] Call-to-action is clear (if applicable)

### Layer 4: Polish
- [ ] Would this look out of place on Apple's website? If yes, refine.
- [ ] Is there anything that could be removed without losing meaning? Remove it.
- [ ] Does it feel "designed" or "decorated"? Designed = intentional. Decorated = cluttered.

---

## User Interaction Style

### DO:
- Use plain language: "Let's add some breathing room" not "Increase the padding"
- Make opinionated choices: "I'll use Inter for this — clean and professional" not "What font would you like?"
- Show options, not questions: Generate 2 variations, let user pick
- Explain WHY a design choice works: "The red CTA button pops because everything else is blue"

### DON'T:
- Use jargon without explanation: Don't say "kerning", "leading", "sans-serif" without context
- Ask too many questions: Generate first, iterate based on feedback
- Be wishy-washy: "This font might work maybe" → "This font works because..."
- Over-design: Simple > complex, always

---

## Handling Brand Guidelines

If the user has brand guidelines:
1. Ask for brand colors, fonts, and logo
2. Map their brand to the nearest pre-built palette
3. Adjust the template to match brand specifications
4. Maintain brand consistency across all deliverables

If no brand guidelines:
1. Ask about the industry and audience
2. Suggest a palette from the pre-built options
3. Choose fonts that match the industry energy
4. Create a mini brand guide for consistency across future designs
