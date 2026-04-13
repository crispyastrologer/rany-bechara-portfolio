# Rany Bechara CV - SpaceX Inspired Design System

Design system for personal portfolio/CV website. Inspired by SpaceX: stark black and white, futuristic, minimal, high-tech aesthetic.

## 1. Visual Theme & Atmosphere

**Mood:** Futuristic, bold, high-tech, professional

**Philosophy:** Full dark theme with stark black background and white text. Minimalist with purposeful use of electric blue accent. Clean lines, bold typography, and high contrast create a cutting-edge aerospace feel.

**Density:** Low density with maximum whitespace. Content breathes. Every element is intentional.

## 2. Color Palette & Roles

| Token | Hex | Usage |
|-------|-----|-------|
| `accent` | `#005288` | Links, highlights, interactive states |
| `accent-light` | `#0A4C78` | Hover states on accent |
| `accent-glow` | `rgba(0, 82, 136, 0.3)` | Subtle glow effects |
| `bg-primary` | `#000000` | Page background |
| `bg-card` | `#0A0A0A` | Card/section backgrounds |
| `bg-card-hover` | `#111111` | Card hover state |
| `text-primary` | `#FFFFFF` | Primary text, headings |
| `text-secondary` | `#999999` | Secondary text, labels |
| `text-muted` | `#666666` | Muted text, placeholders |
| `border` | `#222222` | Subtle borders |
| `border-accent` | `#005288` | Accent borders on focus/hover |

## 3. Typography Rules

**Font Stack:**
```
'Inter', 'SF Pro Display', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif
```

**Type Scale:**

| Element | Size | Weight | Color | Transform |
|---------|------|--------|-------|-----------|
| Name (h1) | 48px | 800 | `#FFFFFF` | uppercase, letter-spacing 8px |
| Title | 14px | 500 | `#005288` | uppercase, letter-spacing 4px |
| Section Title | 10px | 600 | `#666666` | uppercase, letter-spacing 3px |
| Job Title | 16px | 600 | `#FFFFFF` | none |
| Company | 13px | 400 | `#999999` | none |
| Body Text | 14px | 400 | `#CCCCCC` | none, line-height 1.7 |
| Dates | 12px | 500 | `#005288` | none |
| Labels | 10px | 500 | `#666666` | uppercase, letter-spacing 1px |

**Line Height:** 1.7 for body text (generous spacing for readability)

## 4. Component Stylings

### Page Layout
```
Max Width: 1000px
Single column, centered
Background: #000000
No card shadow (flat design)
Border Radius: 0 (sharp corners - SpaceX style)
```

### Main Sections
```
Background: #0A0A0A
Border: 1px solid #222222
Padding: 48px
Margin-bottom: 24px
Hover: background changes to #111111
```

### Header Section
```
Background: transparent
Padding: 64px 48px
Text-align: center
Name: 48px, uppercase, letter-spacing 8px
Title: 14px, uppercase, letter-spacing 4px, accent color
```

### Section Title
```
Font: 10px, uppercase, letter-spacing 3px
Color: #666666
Margin-bottom: 24px
Padding-bottom: 12px
Border-bottom: 1px solid #222222
```

### Contact Row
```
Display: flex
Justify-content: center
Gap: 32px
Flex-wrap: wrap
Icon Color: #005288
Text Color: #999999
Link Color: #FFFFFF (hover: #005288)
```

### Skill Card
```
Background: #0A0A0A
Border: 1px solid #222222
Padding: 16px 12px
Icon Size: 24x24px
Text Size: 10px
Hover:
  - Border-color: #005288
  - Background: #111111
  - cursor: pointer
```

### Interest Tag
```
Background: transparent
Border: 1px solid #333333
Padding: 8px 16px
Font Size: 11px
Hover:
  - Border-color: #005288
  - Color: #005288
```

### Job Entry
```
Border-left: 3px solid #222222
Padding-left: 20px
Margin-bottom: 32px
Hover:
  - Border-left-color: #005288
```

### Education Entry
```
Margin-bottom: 24px
Last-child: margin-bottom 0
```

## 5. Layout Principles

**Grid System:**
- Single centered column (no sidebar)
- Max-width: 1000px
- Generous padding: 48px
- Section spacing: 48px between major sections

**Spacing Scale:**
```
xs: 8px
sm: 12px
md: 16px
lg: 24px
xl: 32px
xxl: 48px
xxxl: 64px
```

**Section Order:**
1. Header (Name + Title + Contact)
2. About / Bio
3. Experience
4. Skills
5. Education
6. Interests

## 6. Depth & Elevation

**Shadows:** None (flat SpaceX aesthetic)

**Border Radius:** 0 (sharp corners throughout)

**Glow Effects:**
```
Accent glow on focus: box-shadow: 0 0 20px rgba(0, 82, 136, 0.3)
```

## 7. Do's and Don'ts

### Do
- Use pure black (#000000) as background
- Use pure white (#FFFFFF) for primary text
- Use electric blue (#005288) for accents and links
- Keep everything flat with subtle borders
- Use generous whitespace
- Use bold, uppercase typography for name/headings
- Add subtle blue glow on interactive focus

### Don't
- Use multiple accent colors - only blue
- Use rounded corners (sharp edges only)
- Use shadows or depth effects
- Use warm colors (orange, yellow, red)
- Use light backgrounds
- Add decorative elements or gradients
- Crowd content - keep it minimal

## 8. Responsive Behavior

**Breakpoints:**
```
Mobile: < 640px
  - Reduce padding to 24px
  - Name size: 32px
  - Contact gap: 16px

Tablet: 640px - 1024px
  - Standard layout with reduced margins

Desktop: > 1024px
  - Full centered layout
```

**Touch Targets:** Minimum 44x44px for interactive elements

## 9. Agent Prompt Guide

**Quick Color Reference:**
```
Primary Background: #000000 (black)
Card Background: #0A0A0A (near black)
Primary Text: #FFFFFF (white)
Accent: #005288 (SpaceX blue)
Secondary Text: #999999 (grey)
Border: #222222 (subtle)
```

**Sample Prompts:**
- "Update the CV design following DESIGN.md - make it more minimal"
- "Add a new skill following the SpaceX-inspired skill card style"
- "Reduce spacing between sections to match DESIGN.md"
- "Change accent color to a different blue tone"
- "Add hover glow effects to interactive elements matching DESIGN.md"
