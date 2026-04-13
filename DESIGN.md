# Rany Bechara CV - SpaceX Inspired Design System

Design system for personal portfolio/CV website. Inspired by SpaceX: stark black and white, futuristic, minimal, high-tech aesthetic with light/dark mode support.

## 1. Visual Theme & Atmosphere

**Mood:** Futuristic, bold, high-tech, professional

**Philosophy:** Full dark theme by default with stark black background and white text. Optional light mode for accessibility. Minimalist with purposeful use of electric blue accent. Clean lines, bold typography, and high contrast create a cutting-edge aerospace feel.

**Density:** Low density with maximum whitespace. Content breathes. Every element is intentional.

## 2. Color Palette & Roles

### CSS Variables Pattern
```css
:root {
    /* Dark Mode (Default) */
    --bg-primary: #000000;
    --bg-card: #0A0A0A;
    --bg-card-hover: #111111;
    --text-primary: #FFFFFF;
    --text-secondary: #999999;
    --text-muted: #666666;
    --accent: #005288;
    --accent-light: #0A4C78;
    --border: #222222;
    --border-accent: #333333;
    --skill-card-bg: #0A0A0A;
    --skill-icon-fill: #bbbbbb;
}

[data-theme="light"] {
    --bg-primary: #ffffff;
    --bg-card: #f8f9fa;
    --bg-card-hover: #f0f1f3;
    --text-primary: #000000;
    --text-secondary: #555555;
    --text-muted: #888888;
    --accent: #005288;
    --accent-light: #003d66;
    --border: #e0e0e0;
    --border-accent: #d0d0d0;
    --skill-card-bg: #f8f9fa;
    --skill-icon-fill: #555555;
}
```

### Color Token Reference

| Token | Dark Mode | Light Mode | Usage |
|-------|-----------|-----------|-------|
| `bg-primary` | `#000000` | `#ffffff` | Page background |
| `bg-card` | `#0A0A0A` | `#f8f9fa` | Card/section backgrounds |
| `bg-card-hover` | `#111111` | `#f0f1f3` | Card hover state |
| `text-primary` | `#FFFFFF` | `#000000` | Primary text, headings |
| `text-secondary` | `#999999` | `#555555` | Secondary text |
| `text-muted` | `#666666` | `#888888` | Muted text, labels |
| `accent` | `#005288` | `#005288` | Links, highlights, interactive |
| `border` | `#222222` | `#e0e0e0` | Subtle borders |
| `border-accent` | `#333333` | `#d0d0d0` | Accent borders |

## 3. Typography Rules

**Font Stack:**
```
'Inter', 'SF Pro Display', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif
```

**Type Scale:**

| Element | Size | Weight | Color | Transform |
|---------|------|--------|-------|-----------|
| Name (h1) | 48px | 800 | `var(--text-primary)` | uppercase, letter-spacing 8px |
| Title | 14px | 500 | `var(--accent)` | uppercase, letter-spacing 4px |
| Section Title | 10px | 600 | `var(--text-muted)` | uppercase, letter-spacing 3px |
| Job Title | 16px | 600 | `var(--text-primary)` | none |
| Company | 13px | 400 | `var(--text-secondary)` | none |
| Body Text | 14px | 400 | `var(--text-secondary)` | none, line-height 1.7 |
| Dates | 12px | 500 | `var(--accent)` | none |
| Labels | 10px | 500 | `var(--text-muted)` | uppercase, letter-spacing 1px |

**Line Height:** 1.7 for body text (generous spacing for readability)

## 4. Component Stylings

### Page Layout
```
Max Width: 1000px
Single column, centered
Background: var(--bg-primary)
No card shadow (flat design)
Border Radius: 0 (sharp corners - SpaceX style)
```

### Theme Toggle Button
```
Position: fixed, top 24px, right 24px
Background: var(--bg-card)
Border: 1px solid var(--border)
Padding: 8px 16px
Icon: 18x18px, fill var(--text-secondary)
Text: 11px, uppercase, letter-spacing 1px
Hover: border-color var(--accent), icon fill var(--accent)
Responsive: Hide text on mobile (< 480px)
```

### Main Sections
```
Background: transparent
Border-bottom: 1px solid var(--border)
Padding: 48px 0
```

### Header Section
```
Background: transparent
Padding: 80px 0 64px
Text-align: center
Border-bottom: 1px solid var(--border)
Name: 48px, uppercase, letter-spacing 8px, var(--text-primary)
Title: 14px, uppercase, letter-spacing 4px, var(--accent)
```

### Section Title
```
Font: 10px, uppercase, letter-spacing 3px
Color: var(--text-muted)
Margin-bottom: 24px
Padding-bottom: 12px
Border-bottom: 1px solid var(--border)
```

### Contact Row
```
Display: flex
Justify-content: center
Gap: 32px
Flex-wrap: wrap
Icon Color: var(--accent)
Text Color: var(--text-secondary)
Link Color: var(--text-primary) (hover: var(--accent))
```

### Skill Card
```
Background: var(--skill-card-bg)
Border: 1px solid var(--border)
Padding: 20px 12px
Icon Size: 28x28px
Icon Fill: var(--skill-icon-fill)
Text Size: 11px
Hover:
  - Border-color: var(--accent)
  - Background: var(--bg-card-hover)
```

### Interest Tag
```
Background: transparent
Border: 1px solid var(--border-accent)
Padding: 10px 20px
Font Size: 12px
Color: var(--text-secondary)
Hover:
  - Border-color: var(--accent)
  - Color: var(--accent)
```

### Job Entry
```
Border-left: 3px solid var(--border)
Padding-left: 24px
Margin-bottom: 40px
Hover:
  - Border-left-color: var(--accent)
```

## 5. Layout Principles

**Grid System:**
- Single centered column (no sidebar)
- Max-width: 1000px
- Generous padding: 48px (container) or 0 with section spacing
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
6. Languages
7. Interests

## 6. Depth & Elevation

**Shadows:** None (flat SpaceX aesthetic)

**Border Radius:** 0 (sharp corners throughout)

**Transitions:** 0.3s ease for theme changes, 0.2s ease for hover states

## 7. Do's and Don'ts

### Do
- Use pure black (#000000) as default dark background
- Use CSS variables for all colors to support theme switching
- Use electric blue (#005288) for accents and links in both themes
- Keep everything flat with subtle borders
- Use generous whitespace
- Use bold, uppercase typography for name/headings
- Add theme toggle button in top-right corner
- Respect system theme preference on first load
- Persist theme choice in localStorage

### Don't
- Use multiple accent colors - only blue
- Use rounded corners (sharp edges only)
- Use shadows or depth effects
- Use warm colors (orange, yellow, red)
- Add decorative elements or gradients
- Crowd content - keep it minimal
- Hardcode colors instead of using CSS variables

## 8. Responsive Behavior

**Breakpoints:**
```
Mobile: < 640px
  - Reduce padding to 24px
  - Name size: 32px, letter-spacing 4px
  - Contact gap: 16px
  - Theme toggle: hide text, show icon only

Tablet: 640px - 1024px
  - Standard layout with reduced margins

Desktop: > 1024px
  - Full centered layout
```

**Touch Targets:** Minimum 44x44px for interactive elements

## 9. Agent Prompt Guide

**Quick Color Reference:**
```
Primary Background (dark): #000000
Primary Background (light): #ffffff
Card Background (dark): #0A0A0A
Card Background (light): #f8f9fa
Primary Text (dark): #FFFFFF
Primary Text (light): #000000
Accent: #005288 (same in both modes)
Secondary Text (dark): #999999
Secondary Text (light): #555555
Border (dark): #222222
Border (light): #e0e0e0
```

**Theme Toggle Implementation:**
```
- Fixed position: top 24px, right 24px
- Use data-theme attribute on body
- Save preference in localStorage
- Check system preference (prefers-color-scheme) on first load
- Smooth transitions (0.3s) for theme changes
```

**Sample Prompts:**
- "Add a theme toggle following DESIGN.md specifications"
- "Update colors to use CSS variables for theme switching"
- "Add light mode styles that complement the dark mode"
- "Implement localStorage persistence for theme preference"
- "Add system preference detection for initial theme"
