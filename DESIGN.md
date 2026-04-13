# Rany Bechara CV Design System

Design system for personal portfolio/CV website. Professional, clean, with dark sidebar and warm orange accents.

## 1. Visual Theme & Atmosphere

**Mood:** Professional, creative, approachable yet polished

**Philosophy:** Split-layout portfolio with dark sidebar for navigation/info and light main area for content. Warm accent color creates visual interest without overwhelming. Minimal decoration with purposeful accent elements.

**Density:** Medium density with generous whitespace. Content-focused without being cramped.

## 2. Color Palette & Roles

| Token | Hex | Usage |
|-------|-----|-------|
| `accent` | `#f5a623` | Highlights, dates, interactive states, links |
| `accent-hover` | `#e09510` | Hover states on accent elements |
| `sidebar-bg` | `#1a1a1a` | Left sidebar background |
| `sidebar-text` | `#cccccc` | Body text on dark background |
| `sidebar-text-muted` | `#888888` | Secondary text, labels on dark |
| `sidebar-border` | `#333333` | Borders on dark background |
| `card-bg` | `#252525` | Skill cards, tag backgrounds on dark |
| `main-bg` | `#ffffff` | Main content area background |
| `main-text` | `#222222` | Headings on light background |
| `main-text-secondary` | `#555555` | Body text on light background |
| `main-border` | `#e0e0e0` | Section dividers on light |
| `page-bg` | `#e8e8e8` | Page background outside card |
| `decorative-yellow` | `linear-gradient(135deg, #f5a623 0%, #f7b955 100%)` | Top-left decorative circle |
| `decorative-grey` | `linear-gradient(135deg, #e0e0e0 0%, #c0c0c0 100%)` | Bottom-right decorative circle |

## 3. Typography Rules

**Font Stack:**
```
'Segoe UI', 'Open Sans', Arial, sans-serif
```

**Type Scale:**

| Element | Size | Weight | Color | Transform |
|---------|------|--------|-------|-----------|
| Name (h1) | 32px | 700 | `#222222` | none, letter-spacing 1px |
| Title | 12px | 600 | `#f5a623` | uppercase, letter-spacing 2px |
| Section Title | 9px | 700 | `#999999` | uppercase, letter-spacing 2px |
| Job Title | 13px | 700 | `#222222` | none |
| Company | 11px | 500 | `#666666` | none |
| Body Text | 11-12px | 400 | `#555555` | none |
| Dates | 11px | 700 | `#f5a623` | none |
| Labels | 8-9px | 700 | `#888888` | uppercase |

**Line Height:** 1.5-1.6 for body text, 1.4 for tighter contexts

## 4. Component Stylings

### Page Layout
```
Max Width: 900px
Grid: 250px sidebar + 1fr main
Shadow: 0 4px 20px rgba(0,0,0,0.08)
Border Radius: 0 (sharp corners)
```

### Sidebar Section
```
Background: #1a1a1a
Padding: 32px 24px
Margin Bottom: 24px
Section Title:
  - Font: 9px, uppercase, letter-spacing 2px
  - Color: #888888
  - Border-bottom: 1px solid #333333
  - Margin-bottom: 12px
  - Padding-bottom: 8px
```

### Contact Item
```
Display: flex
Gap: 10px
Icon Size: 14x14px
Icon Color: #f5a623
Text Color: #cccccc
Link Color: #cccccc (hover: #f5a623)
Margin-bottom: 10px
```

### Skill Card
```
Background: #252525
Border: 1px solid #333333
Padding: 8px 4px
Icon Size: 22x22px
Text Size: 8px
Hover:
  - Border-color: #f5a623
  - Transform: translateY(-2px)
  - cursor: pointer
```

### Interest Tag
```
Background: #252525
Border: 1px solid #333333
Padding: 4px 10px
Font Size: 9px
Hover:
  - Background: #f5a623
  - Color: white
  - Border-color: #f5a623
```

### Job Card
```
Border-left: 2px solid #dddddd
Padding-left: 14px
Margin-bottom: 18px
Hover:
  - Border-left-color: #f5a623
  - Padding-left: 16px
```

### Decorative Circles
```
Top-Left (Yellow):
  Position: fixed, top -60px, left -60px
  Size: 200x200px
  Background: linear-gradient(135deg, #f5a623 0%, #f7b955 100%)
  Opacity: 0.15

Bottom-Right (Grey):
  Position: fixed, bottom -100px, right -100px
  Size: 280x280px
  Background: linear-gradient(135deg, #e0e0e0 0%, #c0c0c0 100%)
  Opacity: 0.3
```

## 5. Layout Principles

**Grid System:**
- Two-column layout: 250px fixed sidebar + flexible main
- Content max-width: 900px
- Page padding: 40px
- Section spacing: 24-28px

**Spacing Scale:**
```
xs: 4px
sm: 8px
md: 12px
lg: 16px
xl: 24px
xxl: 32px
```

**Section Order (Sidebar):**
1. Contact
2. Education
3. Software Skills
4. Languages
5. Interests

**Section Order (Main):**
1. Header (Name + Title)
2. Biography
3. Work Experience

## 6. Depth & Elevation

**Shadows:**
```
Page Card: 0 4px 20px rgba(0,0,0,0.08)
```

**Border Radius:** None (sharp corners throughout)

**Opacity Levels:**
```
Decorative circles: 0.15 - 0.3
Text on dark: 0.5 - 1.0
```

## 7. Do's and Don'ts

### Do
- Use `#f5a623` exclusively for dates, accents, interactive highlights
- Keep sidebar text light (#cccccc) against dark background
- Maintain consistent 2px left border on job cards
- Use gradient fills on decorative circles (not solid colors)
- Keep hover transitions smooth (0.2s ease)

### Don't
- Use blue or other accent colors
- Apply light text on light sidebar background
- Use rounded corners (all sharp)
- Add unnecessary decorative elements beyond the two circles
- Use more than 3 accent colors
- Apply bold weight to body text

## 8. Responsive Behavior

**Breakpoints:**
```
Mobile: < 768px
  - Stack sidebar above main content
  - Reduce page padding to 20px
  - Sidebar becomes full-width with border-bottom

Tablet: 768px - 1024px
  - Use current layout with reduced margins

Desktop: > 1024px
  - Full two-column layout
```

**Touch Targets:** Minimum 44x44px for interactive elements

## 9. Agent Prompt Guide

**Quick Color Reference:**
```
Primary Accent: #f5a623 (orange)
Dark Background: #1a1a1a
Light Background: #ffffff
Text on Dark: #cccccc
Text on Light: #555555
```

**Sample Prompts:**
- "Update the CV design following DESIGN.md - make dates more prominent"
- "Add a new skill to the sidebar following the existing skill card style"
- "Increase spacing between job cards to match DESIGN.md specifications"
- "Change the accent color to a warmer tone while keeping the same saturation"
- "Add hover effects to the interest tags matching DESIGN.md"
