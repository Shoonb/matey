# Matey — Style Guide
> Sourced directly from Figma file: **Matey-Website** (`tctgh2EAd8AMJsVatskiJ5`)
> Last updated: 2026-02-27

---

## 1. Typography

### Font Families

| Role | Family | Weight(s) |
|------|--------|-----------|
| Hero / display headlines | **ABC Ginto Nord Condensed** | 700 (Bold) |
| Footer / UI labels | **ABC Ginto Normal** | 400 (Regular) |
| Body / vision headings | **Nunito** | 400, 900 (Black) |
| Buttons | **Roboto** | 300 (Light), 400 (Regular) |

> **Note:** Figma file uses trial versions ("Unlicensed Trial"). Use the licensed versions of ABC Ginto in production, or confirm with legal before shipping.

### Type Scale

| Token | Family | Size | Weight | Line Height | Color | Usage |
|-------|--------|------|--------|-------------|-------|-------|
| `--text-hero` | Nunito | 58px | 900 (Black) | 68px | `#d3f7d8` | Hero headline — 5 lines, single colour, `text-align: center`, `text-shadow: 0 2.3px 2.3px rgba(0,0,0,0.25)` |
| `--text-vision-lg` | Nunito | 58px | 900 | 68px | `#d3f7d8` | Vision section large heading |
| `--text-nav-tagline` | Nunito | 32px | 600 (SemiBold) | — | `#2d690d` | "DIY made easy." nav tagline — apply `-webkit-font-smoothing: antialiased` to match Figma weight |
| `--text-diy-easy` | Nunito | 32px | 600 (SemiBold) | 44px | `#252423` | "DIY made easy." features heading |
| `--text-cta-heading` | Nunito | 32px | 600 (SemiBold) | 44px | `#ffffff` | "Be The First to Try Matey" CTA card heading — apply `-webkit-font-smoothing: antialiased` |
| `--text-section` | Nunito | 48px | 400 | 65.5px | `#252423` | Section subheadings |
| `--text-btn` | Roboto | 18px | 400 | 48px | `#2d690d` | Primary button label |
| `--text-btn-ghost` | Roboto | 18px | 300 | 48px | `#aef5b7` | Ghost/secondary button label |
| `--text-footer` | ABC Ginto Normal | 18px | 400 | 23.6px | `#ffffff` | Footer legal links |

**Letter spacing:** `0` across all text nodes.

---

## 2. Color Palette

> All colors confirmed from Figma fills. Palette is a monochromatic green system + one warm near-black.

| Token | Hex | Usage |
|-------|-----|-------|
| `--color-bg` | `#f9f9f9` | Page/WAITLIST frame background |
| `--color-green-light` | `#e6f8e9` | Nav background, section backgrounds |
| `--color-green-card` | `#d3f7d8` | Cards, vision body text, "We're here" card border |
| `--color-green-accent` | `#aef5b7` | Hero headline (line 1), CTA button fill, button outer glow border, ghost button text |
| `--color-green-dark` | `#2d690d` | Primary button text, button inner border, "Start a project" text |
| `--color-black` | `#1e2e29` | Page frame border, divider lines, button fill (dark variant) |
| `--color-text-dark` | `#252423` | Section subheadings, body text |
| `--color-white` | `#ffffff` | Footer text, inner shadow highlights |

### "We're here" Glassmorphism Card
| Property | Value |
|----------|-------|
| Fill | `#d3f7d8` at 20% opacity |
| Border | `#d3f7d8` at 12% opacity, 1px inside |
| Inner shadow (highlight) | `rgba(255,255,255,0.35)`, blur 2px, y +1 |
| Inner shadow (depth) | `rgba(0,0,0,0.12)`, blur 6px, y -1 |
| Drop shadow | `rgba(0,0,0,0.12)`, blur 36px, y +14 |
| Background blur | `backdrop-filter: blur(14px)` |

---

## 3. Spacing & Layout

### Grid

| Token | Value |
|-------|-------|
| `--space-unit` | `8px` |
| `--max-content-width` | `1440px` (desktop-only design) |
| `--page-gutter` | `36px` (nav horizontal padding) |

### Spacing Scale

| Multiplier | Value | Common use |
|-----------|-------|-----------|
| 0.5× | `4px` | Tag inner padding, tight icon gaps |
| 1× | `8px` | Icon + label rows |
| 1.25× | `10px` | Page section vertical gap |
| 2× | `16px` | Project card rows |
| 2.5× | `20px` | Button internal gap |
| 3× | `24px` | Card padding, section vertical rhythm |
| 6× | `48px` | CTA strip, join waitlist gap |
| 8× | `64px` | Large content separators, vision top pad |
| 16× | `128px` | Major section separators |

### Section Heights & Padding

| Section | Frame size (W×H) | Padding (T R B L) |
|---------|-----------------|-------------------|
| Header / Nav | 1440 × 134px | `8 36 8 36` |
| Hero / Vision | 1440 × 810px | — |
| DIY Made Easy | 1440 × 641px | `48 0 48 0` |
| Mission / Investor | 1440 × 487px | `24 0 24 0` |
| Projects | 1440 × 362px | — |
| Body section | 1440 × 279px | — |
| Join Waitlist CTA | 1440 × 190px | `48 0 48 0` |
| Full page (WAITLIST) | 1440 × 2938px | `64 0 64 0` (content wrapper) |

### Nav
| Property | Value |
|----------|-------|
| Frame height | `134px` |
| Horizontal padding | `36px` each side |
| Vertical padding | `8px` each side |
| Logo ↔ buttons gap | `600–612px` (space-between layout) |

---

## 4. Components

### Primary Button (pill, filled)
```
font-family:   Roboto
font-size:     18px
font-weight:   400
color:         #2d690d
background:    #1e2e29
border:        1.5px solid #2d690d (inner) + 2px solid #aef5b7 (outer glow)
border-radius: 64px (full pill)
padding:       20px 16px
line-height:   48px
```

### Ghost / Secondary Button
```
font-family:   Roboto
font-size:     18px
font-weight:   300
color:         #aef5b7
background:    transparent
border:        none
line-height:   48px
```

### Tag / Badge Chip
```
border-radius: 8px
padding:       4px
background:    --color-green-accent or --color-green-card
```

### "We're here" Glassmorphism Card
```
width:              591px
padding:            24px
border-radius:      8.9px
background:         rgba(#d3f7d8, 0.20)
border:             1px solid rgba(#d3f7d8, 0.12)
backdrop-filter:    blur(14px)
box-shadow:         inset 0 1px 2px rgba(255,255,255,0.35),
                    inset 0 -1px 6px rgba(0,0,0,0.12),
                    0 14px 36px rgba(0,0,0,0.12)
item-spacing:       8.9px (flex gap)
```

---

## 5. Effects & Shadows

| Effect | Value | Used on |
|--------|-------|---------|
| Hero text drop shadow | `0 2.3px 2.3px rgba(0,0,0,0.25)` | Hero headline text |
| Card drop shadow | `0 14px 36px rgba(0,0,0,0.12)` | "We're here" card |
| Card inner highlight | `inset 0 1px 2px rgba(255,255,255,0.35)` | "We're here" card |
| Card inner depth | `inset 0 -1px 6px rgba(0,0,0,0.12)` | "We're here" card |
| Card backdrop blur | `backdrop-filter: blur(14px)` | "We're here" card |

---

## 6. Borders & Dividers

| Element | Color | Weight |
|---------|-------|--------|
| Page outer frame | `#1e2e29` | 1px inside |
| "We're here" card | `#d3f7d8` @ 12% | 1px inside |
| Section divider lines | `#1e2e29` | 0.5px center |
| Primary button inner | `#2d690d` | 1.5px inside |
| Primary button outer glow | `#aef5b7` | 2px inside |

---

## 7. Images & Assets

| Location | Description | Local path |
|----------|-------------|------------|
| Hero / Vision full-bleed | Woman celebrating (warm tones) — `object-fit: cover; object-position: center top` to anchor raised arms at top of 810px frame | `Assets/SVGs/images/imgs (hero + footer)/vision-img.svg` |
| Footer | Footer background image | `Assets/SVGs/images/imgs (hero + footer)/footer-img.svg` |
| Apartment scan | Floor plan / apt illustration | `Assets/SVGs/images/apt/apt.svg` |
| Scan start state | Scan UI illustration | `Assets/SVGs/images/scan/SCAN-start.svg` |
| Scan end state | Scan UI illustration | `Assets/SVGs/images/scan/SCAN-end.svg` |
| Coffee table — cube | Product photo | `Assets/SVGs/images/coffee_tables/coffee_table-cube.png` |
| Coffee table — chunky legs | Product photo | `Assets/SVGs/images/coffee_tables/coffee_table-chunky legs.png` |
| Coffee table — japanese | Product photo | `Assets/SVGs/images/coffee_tables/coffee_table-japanese.png` |
| Logo (wordmark) | SVG vector | `Assets/SVGs/logo/Matey-logo.svg` |

---

## 8. Icons

All icons located in `Assets/SVGs/icons/`:

| File | Usage |
|------|-------|
| `icon-scan.svg` | Scan feature |
| `icon-arrow_right.svg` | CTAs, navigation |
| `Icon-arrow_down.svg` | Dropdowns / scroll |
| `icon-list.svg` | Project list feature |
| `icon-shop.svg` | Shop feature |
| `icon-play.svg` | Video DIY section |
| `icon-community.svg` | Community feature |

---

## 9. Layout Notes

- **Desktop-only**: All Figma frames are `1440px` wide. No mobile breakpoints defined yet.
- **Vertical scroll**: The WAITLIST frame has `overflowDirection: VERTICAL_SCROLLING` — page scrolls vertically.
- **Section rhythm**: Main sections are separated by `10px` itemSpacing at the page level; internal spacing jumps to `64–128px` for major content blocks.
- **Hero headline**: 5 lines, `display: block; text-align: center`, natural `68px` line-height — no negative gap.
- **Two-column at 716px**: Many content sections split into `716px` half-columns within the 1440px frame.
