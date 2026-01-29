# 🎨 TalosPro Design Quick Reference Card

**Print this or keep it open while designing/coding**

---

## Colors (Copy-Paste Ready)

```css
/* PRIMARY - Use for brand, main CTAs */
#7c3aed  /* Primary 500 - main purple */
#a78bfa  /* Primary 400 - light purple */
#6d28d9  /* Primary 600 - dark purple */

/* ACCENT - Use for highlights, links */
#60a5fa  /* Accent 500 - sky blue */
#3b82f6  /* Accent 600 - bright blue */

/* BACKGROUNDS - Dark theme */
#0d0d0f  /* Dark 950 - page background */
#1a1a1f  /* Dark 900 - cards */
#27272f  /* Dark 800 - elevated surfaces */
#34343f  /* Dark 700 - borders */

/* STATUS */
#10b981  /* Success - green */
#f59e0b  /* Warning - orange */
#ef4444  /* Danger - red */
```

---

## Typography

```css
/* FONT */
font-family: 'Inter', system-ui, sans-serif;

/* SIZES */
12px  text-xs    /* Fine print */
14px  text-sm    /* Secondary text */
16px  text-base  /* Body (default) */
20px  text-xl    /* Emphasized */
24px  text-2xl   /* H3 */
30px  text-3xl   /* H2, H1 mobile */
36px  text-4xl   /* H1 desktop */

/* WEIGHTS */
400  font-normal    /* Body */
500  font-medium    /* Emphasis */
600  font-semibold  /* Subheadings */
700  font-bold      /* Headings */
```

---

## Spacing (4px base)

```
0   0px     space-0   gap-0
1   4px     space-1   gap-1
2   8px     space-2   gap-2
3   12px    space-3   gap-3
4   16px    space-4   gap-4    ← Common
6   24px    space-6   gap-6    ← Common
8   32px    space-8   gap-8
12  48px    space-12  gap-12   ← Sections
16  64px    space-16  gap-16   ← Hero
```

---

## Common Patterns

### Button (Primary)
```html
class="px-6 py-3 rounded-lg font-semibold bg-gradient-to-br from-primary-500 to-indigo-600 text-white shadow-lg hover:-translate-y-0.5 transition-all"
```

### Card (Glass)
```html
class="p-6 rounded-xl bg-dark-900/80 border border-white/10 backdrop-blur-xl shadow-lg hover:-translate-y-1 transition-all"
```

### Input
```html
class="w-full px-4 py-3 rounded-lg bg-dark-900/50 border border-dark-700 text-white focus:border-accent-500 focus:ring-4 focus:ring-accent-500/10 transition-all"
```

### Text Colors
```html
text-white           /* Headings, emphasis (100%) */
text-white/87        /* Body text (87%) */
text-white/70        /* Secondary text (70%) */
text-white/50        /* Muted text (50%) */
text-white/40        /* Placeholders (40%) */
```

---

## Effects

### Glassmorphism
```css
background: rgba(26, 26, 31, 0.8);
backdrop-filter: blur(20px);
border: 1px solid rgba(255, 255, 255, 0.1);
```

### Gradient (Purple→Blue)
```css
background: linear-gradient(135deg, #7c3aed 0%, #60a5fa 100%);
```

### Shadow (Subtle)
```css
box-shadow: 0 4px 14px rgba(124, 58, 237, 0.2);
```

### Hover Lift
```css
transition: all 0.3s ease;
hover: transform translateY(-2px);
```

---

## Responsive

```
< 640px   Mobile       (icon only logo)
≥ 640px   sm:          (show horizontal logo)
≥ 768px   md:          (2-column grids)
≥ 1024px  lg:          (3-column grids)
≥ 1280px  xl:          (expanded layouts)
```

---

## Logo Usage

```
Icon Only:
- Mobile headers: h-8 (32px)
- Favicons: 32×32px min
- Social avatars: platform size

Horizontal:
- Desktop headers: h-6 (24px)
- Marketing: h-8 to h-10
- Minimum: h-6 (24px)

Clear space: 1/4 logo height
```

---

## Component Sizes

### Buttons
```
Small:  px-4 py-2 text-sm
Medium: px-6 py-3 text-base  ← Default
Large:  px-8 py-4 text-lg
```

### Cards
```
Padding: p-6 (24px)  ← Default
Compact: p-4 (16px)
Spacious: p-8 (32px)
```

### Icons
```
Small:  w-4 h-4 (16px)  - inline
Medium: w-6 h-6 (24px)  ← Default
Large:  w-8 h-8 (32px)  - features
Hero:   w-12 h-12 (48px) - marketing
```

---

## Accessibility

```
WCAG AA Requirements:
Normal text:  4.5:1 contrast  ✅ White on #0d0d0f (21:1)
Large text:   3:1 contrast    ✅ All combinations pass
Focus states: Required        ✅ Blue ring on focus

Always include:
- Focus rings (keyboard nav)
- Alt text (images)
- ARIA labels (interactive)
```

---

## Status Badge Colors

```html
<!-- Success (Green) -->
class="bg-success/10 text-success border-success/20"

<!-- Warning (Orange) -->
class="bg-warning/10 text-warning border-warning/20"

<!-- Danger (Red) -->
class="bg-danger/10 text-danger border-danger/20"

<!-- Info (Blue) -->
class="bg-accent-500/10 text-accent-500 border-accent-500/20"
```

---

## Grid Layouts

```html
<!-- 3-Column Responsive -->
class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6"

<!-- 4-Column Stats -->
class="grid grid-cols-2 lg:grid-cols-4 gap-4"

<!-- Sidebar + Main -->
class="grid grid-cols-1 lg:grid-cols-[240px_1fr] gap-6"
```

---

## Animation Timings

```css
transition: 0.2s ease;           /* Fast (hover feedback) */
transition: 0.3s ease;           /* Standard (default) */
transition: 0.5s ease;           /* Slow (shine effects) */
cubic-bezier(0.4, 0, 0.2, 1);   /* Smooth (preferred) */
```

---

## Don'ts ❌

- ❌ Don't use solid black (#000000) - use #0d0d0f
- ❌ Don't stretch logos - maintain aspect ratio
- ❌ Don't use colors outside the palette
- ❌ Don't skip hover states on interactive elements
- ❌ Don't use less than 16px font size for body text
- ❌ Don't forget focus states for accessibility
- ❌ Don't use raster logos when SVG is available

---

## Do's ✅

- ✅ Use Inter font family
- ✅ Mobile-first responsive design
- ✅ Glassmorphism on elevated surfaces
- ✅ Consistent 4px spacing grid
- ✅ Purple for primary actions
- ✅ Blue for secondary highlights
- ✅ Test on dark backgrounds (our default)
- ✅ Add subtle hover animations

---

## Most Common Classes

```html
<!-- Flex center -->
class="flex items-center justify-center"

<!-- Stack vertically -->
class="flex flex-col space-y-4"

<!-- Horizontal split -->
class="flex items-center justify-between"

<!-- Hide on mobile, show on desktop -->
class="hidden sm:block"

<!-- Full width -->
class="w-full"

<!-- Rounded corners -->
class="rounded-lg"   (8px - default)
class="rounded-xl"   (12px - cards)
class="rounded-2xl"  (16px - modals)

<!-- Transition -->
class="transition-all duration-300"
```

---

**Need more details? See:**
- Full guide: `~/dev/BRAND_GUIDELINE.md`
- Code examples: `~/dev/brand-assets/COMPONENT-EXAMPLES.md`
- Assets: `~/dev/brand-assets/`

**Questions? Ask Sunny or Pixel**

---

*Keep this reference handy while building!*
