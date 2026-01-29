# 💎 TalosPro Brand Guideline
**Version 1.0** | Last Updated: January 2025

> **Purpose:** This guideline ensures visual consistency across all TalosPro products, marketing materials, and communications. Follow these standards to maintain our brand identity.

---

## 1. Brand Overview

### Mission
Empower individuals and businesses to unlock their wealth potential through AI-driven financial intelligence.

### Vision
Become the most trusted AI financial advisor, making sophisticated wealth management accessible to everyone.

### Brand Personality
- **Modern** - Cutting-edge technology, sleek design, forward-thinking
- **Tech-Forward** - AI-first, innovative, data-driven
- **Trustworthy** - Professional, secure, reliable, transparent
- **Premium** - High-quality, polished, attention to detail
- **Approachable** - User-friendly, educational, supportive

### Voice & Tone

#### Voice (Consistent Across All Content)
- **Clear & Direct** - No jargon unless necessary; explain complex concepts simply
- **Confident** - We know what we're talking about
- **Friendly** - Professional but warm, never robotic
- **Empowering** - Focus on what users can achieve

#### Tone (Adapts to Context)
- **Marketing/Landing Pages** - Inspiring, ambitious, benefit-focused
- **Product UI** - Helpful, concise, actionable
- **Support/Help** - Patient, educational, reassuring
- **Technical Docs** - Precise, thorough, structured

**Examples:**
```
✅ Good: "Your AI financial advisor is ready. Let's build your wealth."
❌ Bad: "Utilizing advanced machine learning algorithms to optimize portfolio allocation."

✅ Good: "We found 3 ways to save you $2,400 this year."
❌ Bad: "Our system has identified several optimization opportunities."
```

---

## 2. Logo System

### Primary Logo Assets

**Icon Only (Crystal)**
- **File:** `/logo.svg`
- **Fallback URL:** `https://talospro.ai/logos-final/talos-crystal-gradient.svg`
- **Use Case:** Favicons, app icons, social media avatars, mobile headers

**Horizontal Logo**
- **File:** `talos-logo-horizontal-white.svg`
- **Fallback URL:** `https://talospro.ai/logos-final/talos-logo-horizontal-white.svg`
- **Use Case:** Desktop headers, marketing materials, email signatures

### Logo Anatomy

The TalosPro crystal represents:
- **Faceted geometry** - Multi-dimensional financial insights
- **Gradient warmth** - Purple (technology) → Coral (growth)
- **Clarity & precision** - Cut gem = refined AI intelligence
- **Depth** - Multi-layered facets = sophisticated analysis

### Usage Rules

#### When to Use Which Logo

| Context | Logo Type | Size | Notes |
|---------|-----------|------|-------|
| Mobile (<640px) | Icon only | h-8 (32px) | Save space |
| Desktop (≥640px) | Horizontal | h-6 (24px) | Full branding |
| Favicon | Icon only | 32x32px | Simplified if needed |
| Social Media Avatar | Icon only | Platform-specific | No text |
| Email Signature | Horizontal | h-10 (40px) | Professional |
| Print Materials | Horizontal | ≥1 inch tall | High-res export |

#### Sizing Standards

**Icon Logo**
- **Minimum Size:** 24px × 24px (web), 0.5 inch (print)
- **Recommended Web:** h-8 (32px), h-10 (40px), h-12 (48px)
- **Maximum:** No limit, SVG scales infinitely

**Horizontal Logo**
- **Minimum Size:** h-6 (24px) / 0.75 inch
- **Recommended Web:** h-6 to h-10
- **Maximum:** h-16 (64px) for hero sections

#### Clear Space

Maintain minimum clear space around logo equal to **1/4 of logo height**

```
┌────────────────────────┐
│                        │
│   ┌─────────────┐      │
│   │    LOGO     │      │ ← Clear space = 1/4 logo height
│   └─────────────┘      │
│                        │
└────────────────────────┘
```

### Logo Don'ts

❌ **Never:**
- Stretch or distort the logo (maintain aspect ratio)
- Change colors (always use original gradient)
- Add drop shadows, outlines, or effects
- Rotate or skew the logo
- Place on busy backgrounds without a backdrop
- Use low-resolution raster versions when SVG is available
- Recreate or redraw the logo
- Alter spacing between icon and text in horizontal version

✅ **Instead:**
- Always use provided SVG files
- Use white/dark backdrop on photos: `bg-dark-950/80 backdrop-blur-md`
- Scale proportionally

---

## 3. Color Palette

### Primary Colors

```css
/* Purple - Primary Brand Color */
--primary-500: #7c3aed  /* Main purple */
--primary-600: #6d28d9  /* Darker purple */
--primary-700: #5b21b6  /* Deep purple */

/* Lighter variants (generated) */
--primary-400: #a78bfa  /* Light purple */
--primary-300: #c4b5fd  /* Very light purple */

/* Blue - Accent Color */
--accent-500: #60a5fa   /* Sky blue */
--accent-600: #3b82f6   /* Bright blue */
```

**Color Swatches:**

```
████ #7c3aed  Primary Purple (main)
████ #6d28d9  Primary Purple Dark
████ #5b21b6  Primary Purple Deep
████ #a78bfa  Primary Purple Light
████ #60a5fa  Accent Blue
████ #3b82f6  Accent Blue Dark
```

### Neutral Colors (Dark Theme)

```css
/* Background Layers */
--dark-950: #0d0d0f     /* Main background */
--dark-900: #1a1a1f     /* Elevated surfaces */
--dark-800: #27272f     /* Cards, panels */
--dark-700: #34343f     /* Borders */

/* Text & UI Elements */
--dark-500: #6b6b7b     /* Muted text */
--dark-400: #9090a0     /* Secondary text */
--dark-300: #b5b5c5     /* Primary text */
--white: #ffffff        /* Headings, emphasis */
```

### Semantic Colors

```css
/* Status & Feedback */
--success: #10b981      /* Green - success, profit, positive */
--warning: #f59e0b      /* Orange - warning, caution */
--danger: #ef4444       /* Red - error, loss, negative */
--info: #60a5fa         /* Blue - info, neutral highlight */
```

### Usage Guidelines

| Color | Use For | Don't Use For |
|-------|---------|---------------|
| Primary Purple (#7c3aed) | Primary CTAs, brand elements, active states, links | Body text, backgrounds (too vibrant) |
| Accent Blue (#60a5fa) | Secondary CTAs, highlights, hover states, data viz | Primary branding (that's purple) |
| Dark 950 (#0d0d0f) | Page backgrounds, darkest surfaces | Text (too dark, no contrast) |
| Dark 800-900 | Cards, panels, elevated surfaces | Buttons (too subtle) |
| Success Green | Profit, gains, success messages, positive trends | Neutral actions |
| Danger Red | Losses, errors, destructive actions, negative trends | General highlights |

### Color Combinations

**Recommended Pairings:**
```css
/* High Contrast (Accessibility) */
Background: #0d0d0f  Text: #ffffff       ✅ WCAG AAA
Background: #1a1a1f  Text: #ffffff       ✅ WCAG AAA
Background: #7c3aed  Text: #ffffff       ✅ WCAG AA

/* Subtle Elevation */
Background: #0d0d0f  Card: #1a1a1f  Border: rgba(255,255,255,0.1)

/* Interactive Elements */
Default: bg-white/5  Hover: bg-white/10  Active: bg-purple-600

/* Gradients */
Hero: linear-gradient(135deg, #7c3aed 0%, #60a5fa 100%)
Button: linear-gradient(135deg, #7c3aed 0%, #6366f1 100%)
```

---

## 4. Typography

### Font Family

**Primary Font:** [Inter](https://fonts.google.com/specimen/Inter)
- Modern, highly legible, designed for screens
- Excellent character distinction (1, l, I easily differentiated)
- Wide weight range (300–800)

**Installation:**
```html
<!-- Google Fonts -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
```

```css
/* CSS */
font-family: 'Inter', system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
```

**Fallback Stack:**
```css
font-family: 'Inter', system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Roboto', 'Oxygen', 'Ubuntu', 'Cantarell', 'Helvetica Neue', sans-serif;
```

### Font Sizes (Tailwind Scale)

```css
text-xs:   12px  /* Fine print, badges */
text-sm:   14px  /* Secondary text, captions */
text-base: 16px  /* Body text (default) */
text-lg:   18px  /* Emphasized body, subheadings */
text-xl:   20px  /* Large text, small headings */
text-2xl:  24px  /* H3 */
text-3xl:  30px  /* H2, H1 on mobile */
text-4xl:  36px  /* H1 on desktop */
text-5xl:  48px  /* Hero headings */
```

### Heading Styles

```css
/* H1 - Page Titles */
.h1 {
  font-size: 30px;      /* text-3xl */
  font-weight: 700;     /* font-bold */
  letter-spacing: -0.02em;
  line-height: 1.2;
  color: #ffffff;
}

/* H2 - Section Headings */
.h2 {
  font-size: 24px;      /* text-2xl */
  font-weight: 700;     /* font-bold */
  letter-spacing: -0.01em;
  line-height: 1.3;
  color: #ffffff;
}

/* H3 - Subsection Headings */
.h3 {
  font-size: 20px;      /* text-xl */
  font-weight: 600;     /* font-semibold */
  letter-spacing: -0.01em;
  line-height: 1.4;
  color: #ffffff;
}

/* Body Text */
body {
  font-size: 16px;      /* text-base */
  font-weight: 400;     /* font-normal */
  line-height: 1.6;
  color: rgba(255, 255, 255, 0.87);
}

/* Small Text */
.text-sm {
  font-size: 14px;
  line-height: 1.5;
  color: rgba(255, 255, 255, 0.7);
}
```

### Weight Usage

| Weight | Value | Use For |
|--------|-------|---------|
| Light | 300 | Large display text (sparingly) |
| Regular | 400 | Body text, descriptions |
| Medium | 500 | Emphasized text, labels |
| Semibold | 600 | Subheadings, button text |
| Bold | 700 | Headings, important CTAs |
| Extrabold | 800 | Hero text, marketing (sparingly) |

### Letter Spacing

```css
/* Tighter for headings (improves density) */
letter-spacing: -0.02em;  /* H1 */
letter-spacing: -0.01em;  /* H2, H3 */

/* Normal for body */
letter-spacing: normal;   /* Body text */
```

---

## 5. UI Components

### Buttons

#### Primary Button
**Use:** Main CTAs, primary actions
```html
<button class="btn-primary">Get Started</button>
```

```css
.btn-primary {
  background: linear-gradient(135deg, #7c3aed 0%, #6366f1 100%);
  color: #ffffff;
  padding: 12px 24px;
  border-radius: 8px;
  font-weight: 600;
  font-size: 16px;
  box-shadow: 0 4px 14px rgba(124, 58, 237, 0.4);
  transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
  position: relative;
  overflow: hidden;
}

.btn-primary:hover {
  transform: translateY(-2px);
  box-shadow: 0 8px 24px rgba(124, 58, 237, 0.5);
}

.btn-primary:active {
  transform: translateY(0);
}

/* Shine effect on hover */
.btn-primary::before {
  content: '';
  position: absolute;
  top: 0;
  left: -100%;
  width: 100%;
  height: 100%;
  background: linear-gradient(
    90deg,
    transparent,
    rgba(255, 255, 255, 0.2),
    transparent
  );
  transition: left 0.5s ease;
}

.btn-primary:hover::before {
  left: 100%;
}
```

#### Secondary Button
**Use:** Secondary actions, less emphasis
```css
.btn-secondary {
  background: rgba(255, 255, 255, 0.05);
  border: 1px solid rgba(255, 255, 255, 0.1);
  color: #ffffff;
  padding: 12px 24px;
  border-radius: 8px;
  font-weight: 600;
  transition: all 0.3s ease;
}

.btn-secondary:hover {
  background: rgba(255, 255, 255, 0.1);
  border-color: rgba(255, 255, 255, 0.2);
  transform: translateY(-2px);
}
```

#### Ghost Button
**Use:** Tertiary actions, subtle interactions
```css
.btn-ghost {
  background: rgba(124, 58, 237, 0.05);
  border: 1px solid rgba(124, 58, 237, 0.2);
  color: #a78bfa;
  padding: 12px 24px;
  border-radius: 8px;
  font-weight: 600;
  transition: all 0.3s ease;
}

.btn-ghost:hover {
  background: rgba(124, 58, 237, 0.15);
  border-color: rgba(167, 139, 250, 0.4);
  box-shadow: 0 0 20px rgba(124, 58, 237, 0.3);
}
```

### Cards

#### Standard Glass Card
```html
<div class="card">
  <h3>Card Title</h3>
  <p>Card content...</p>
</div>
```

```css
.card {
  background: linear-gradient(
    135deg,
    rgba(26, 26, 31, 0.9) 0%,
    rgba(17, 17, 22, 0.95) 100%
  );
  border: 1px solid rgba(255, 255, 255, 0.1);
  border-radius: 12px;
  padding: 24px;
  box-shadow: 
    0 8px 32px rgba(0, 0, 0, 0.3),
    inset 0 1px 0 rgba(255, 255, 255, 0.1);
  backdrop-filter: blur(20px);
  transition: all 0.3s ease;
}

.card:hover {
  border-color: rgba(167, 139, 250, 0.3);
  box-shadow: 
    0 12px 48px rgba(124, 58, 237, 0.2),
    inset 0 1px 0 rgba(255, 255, 255, 0.15);
  transform: translateY(-2px);
}
```

#### Stat Card with Gradient Accent
```css
.stat-card {
  position: relative;
  overflow: hidden;
  /* Same base styles as .card */
}

.stat-card::after {
  content: '';
  position: absolute;
  top: 0;
  right: 0;
  width: 100px;
  height: 100px;
  background: radial-gradient(
    circle at center,
    rgba(124, 58, 237, 0.15) 0%,
    transparent 70%
  );
  pointer-events: none;
}
```

### Form Inputs

```html
<input type="text" class="input" placeholder="Enter amount...">
```

```css
.input {
  background: rgba(26, 26, 31, 0.5);
  border: 1px solid #34343f;
  border-radius: 8px;
  padding: 12px 16px;
  font-size: 16px;
  color: #ffffff;
  transition: all 0.3s ease;
}

.input:focus {
  outline: none;
  border-color: #60a5fa;
  box-shadow: 0 0 0 3px rgba(96, 165, 250, 0.1);
  background: rgba(26, 26, 31, 0.7);
}

.input::placeholder {
  color: rgba(255, 255, 255, 0.4);
}
```

### Tables

```css
table {
  width: 100%;
  border-collapse: separate;
  border-spacing: 0;
}

/* Sticky Header */
table thead th {
  position: sticky;
  top: 0;
  background: linear-gradient(
    180deg,
    rgba(32, 33, 35, 0.95) 0%,
    rgba(32, 33, 35, 0.9) 100%
  );
  backdrop-filter: blur(10px);
  padding: 16px;
  text-align: left;
  font-weight: 600;
  font-size: 14px;
  color: rgba(255, 255, 255, 0.7);
  border-bottom: 1px solid rgba(124, 58, 237, 0.2);
  z-index: 10;
}

/* Zebra Striping */
table tbody tr:nth-child(even) {
  background: linear-gradient(
    90deg,
    rgba(124, 58, 237, 0.03) 0%,
    rgba(124, 58, 237, 0.01) 100%
  );
}

/* Hover Effect */
table tbody tr {
  transition: all 0.2s ease;
}

table tbody tr:hover {
  background: linear-gradient(
    90deg,
    rgba(124, 58, 237, 0.1) 0%,
    rgba(124, 58, 237, 0.05) 100%
  );
  box-shadow: inset 0 0 0 1px rgba(167, 139, 250, 0.2);
  transform: scale(1.005);
}

table tbody td {
  padding: 16px;
  border-bottom: 1px solid rgba(255, 255, 255, 0.05);
}
```

### Modal/Dialog

```html
<div class="modal-overlay">
  <div class="modal">
    <h2>Modal Title</h2>
    <p>Content...</p>
    <button class="btn-primary">Confirm</button>
  </div>
</div>
```

```css
.modal-overlay {
  position: fixed;
  inset: 0;
  background: rgba(0, 0, 0, 0.8);
  backdrop-filter: blur(8px);
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: 50;
}

.modal {
  background: linear-gradient(
    135deg,
    rgba(26, 26, 31, 0.95) 0%,
    rgba(17, 17, 22, 0.98) 100%
  );
  border: 1px solid rgba(255, 255, 255, 0.15);
  border-radius: 16px;
  padding: 32px;
  max-width: 500px;
  width: 90%;
  box-shadow: 
    0 24px 64px rgba(0, 0, 0, 0.5),
    inset 0 1px 0 rgba(255, 255, 255, 0.1);
  backdrop-filter: blur(40px);
}
```

---

## 6. Visual Effects

### Glassmorphism

**Light Glass** (subtle elevation)
```css
.glass-light {
  background: rgba(26, 26, 31, 0.6);
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.05);
}
```

**Standard Glass** (cards, panels)
```css
.glass {
  background: rgba(26, 26, 31, 0.8);
  backdrop-filter: blur(20px);
  border: 1px solid rgba(255, 255, 255, 0.1);
}
```

**Heavy Glass** (modals, overlays)
```css
.glass-heavy {
  background: rgba(26, 26, 31, 0.95);
  backdrop-filter: blur(40px);
  border: 1px solid rgba(255, 255, 255, 0.15);
}
```

### Gradients

**Purple to Blue** (hero sections, primary CTAs)
```css
background: linear-gradient(135deg, #7c3aed 0%, #60a5fa 100%);
```

**Purple Shades** (buttons, highlights)
```css
background: linear-gradient(135deg, #7c3aed 0%, #6366f1 100%);
```

**Text Gradient**
```css
.gradient-text {
  background: linear-gradient(135deg, #a78bfa 0%, #60a5fa 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}
```

**Background Mesh** (page backgrounds)
```css
.mesh-gradient {
  background: 
    radial-gradient(at 40% 20%, rgba(124, 58, 237, 0.15) 0px, transparent 50%),
    radial-gradient(at 80% 0%, rgba(59, 130, 246, 0.12) 0px, transparent 50%),
    radial-gradient(at 0% 50%, rgba(6, 182, 212, 0.1) 0px, transparent 50%),
    #0d0d0f;
}
```

### Shadows

**Subtle Elevation** (cards at rest)
```css
box-shadow: 0 4px 14px rgba(124, 58, 237, 0.2);
```

**Strong Elevation** (modals, hover states)
```css
box-shadow: 0 12px 48px rgba(124, 58, 237, 0.3);
```

**Multi-Layer Shadow** (premium elements)
```css
box-shadow: 
  0 8px 32px rgba(0, 0, 0, 0.3),
  inset 0 1px 0 rgba(255, 255, 255, 0.1);
```

**Glow Effect** (interactive elements)
```css
box-shadow: 
  0 0 20px rgba(124, 58, 237, 0.4),
  0 0 40px rgba(124, 58, 237, 0.2);
```

### Animations

**Standard Transition**
```css
transition: all 0.3s ease;
/* Or for more control: */
transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
```

**Hover Lift**
```css
transform: translateY(-2px);
```

**Shimmer Effect** (loading states)
```css
@keyframes shimmer {
  0% { background-position: -1000px 0; }
  100% { background-position: 1000px 0; }
}

.shimmer {
  background: linear-gradient(
    90deg,
    transparent,
    rgba(255, 255, 255, 0.1),
    transparent
  );
  background-size: 1000px 100%;
  animation: shimmer 2s infinite;
}
```

**Pulse Ring** (status indicators)
```css
@keyframes pulse-ring {
  0% {
    transform: scale(0.8);
    opacity: 1;
  }
  100% {
    transform: scale(2);
    opacity: 0;
  }
}

.status-online::before {
  content: '';
  position: absolute;
  inset: -4px;
  border-radius: 50%;
  background: #10b981;
  animation: pulse-ring 1.5s cubic-bezier(0.4, 0, 0.6, 1) infinite;
}
```

---

## 7. Responsive Breakpoints

### Tailwind Breakpoints
```css
/* Mobile-first approach */
sm:  640px   /* Small tablets, large phones (landscape) */
md:  768px   /* Tablets */
lg:  1024px  /* Small laptops */
xl:  1280px  /* Desktops */
2xl: 1536px  /* Large desktops */
```

### Logo Responsiveness
```jsx
{/* Icon only on mobile, icon + text on desktop */}
<div className="flex items-center gap-3">
  <img src="/logo.svg" alt="TalosPro" className="h-8" />
  <span className="hidden sm:block text-xl font-bold">TalosPro</span>
</div>
```

### Typography Scaling
```html
<!-- H1: 30px mobile → 36px desktop -->
<h1 class="text-3xl lg:text-4xl font-bold">Heading</h1>

<!-- Body: 14px mobile → 16px desktop -->
<p class="text-sm md:text-base">Body text...</p>
```

### Grid Layouts
```html
<!-- 1 column mobile → 2 columns tablet → 3 columns desktop -->
<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
  <!-- Cards -->
</div>
```

---

## 8. Spacing System

### Tailwind Scale (4px base)
```css
0:  0px
1:  4px    /* Tight spacing */
2:  8px    /* Compact */
3:  12px   /* Comfortable */
4:  16px   /* Default */
6:  24px   /* Generous */
8:  32px   /* Spacious */
12: 48px   /* Section spacing */
16: 64px   /* Hero spacing */
```

### Common Patterns
```html
<!-- Card Padding -->
<div class="p-6">...</div>          <!-- 24px all sides -->
<div class="p-4 md:p-6">...</div>   <!-- 16px mobile, 24px desktop -->

<!-- Stack Spacing (vertical) -->
<div class="space-y-4">...</div>    <!-- 16px between children -->
<div class="space-y-6">...</div>    <!-- 24px between children -->

<!-- Grid Gaps -->
<div class="grid gap-4">...</div>   <!-- 16px grid gap -->
<div class="grid gap-6">...</div>   <!-- 24px grid gap -->

<!-- Section Margins -->
<section class="mb-12">...</section>  <!-- 48px bottom margin -->
<section class="py-16">...</section>  <!-- 64px vertical padding -->
```

---

## 9. Component Examples

### Complete Button Component (React)
```jsx
export function Button({ 
  variant = 'primary', 
  size = 'md', 
  children, 
  ...props 
}) {
  const baseStyles = "font-semibold rounded-lg transition-all duration-300 relative overflow-hidden";
  
  const variants = {
    primary: "bg-gradient-to-br from-primary-500 to-indigo-600 text-white shadow-lg shadow-primary-500/40 hover:shadow-xl hover:shadow-primary-500/50 hover:-translate-y-0.5 active:translate-y-0",
    secondary: "bg-white/5 border border-white/10 text-white hover:bg-white/10 hover:border-white/20 hover:-translate-y-0.5",
    ghost: "bg-primary-500/5 border border-primary-500/20 text-primary-300 hover:bg-primary-500/15 hover:border-primary-400/40 hover:shadow-lg hover:shadow-primary-500/30"
  };
  
  const sizes = {
    sm: "px-4 py-2 text-sm",
    md: "px-6 py-3 text-base",
    lg: "px-8 py-4 text-lg"
  };
  
  return (
    <button 
      className={`${baseStyles} ${variants[variant]} ${sizes[size]}`}
      {...props}
    >
      {variant === 'primary' && (
        <span className="absolute inset-0 -left-full group-hover:left-full transition-all duration-500 bg-gradient-to-r from-transparent via-white/20 to-transparent" />
      )}
      {children}
    </button>
  );
}
```

### Complete Card Component (React)
```jsx
export function Card({ hover = true, gradient = false, children, className = '' }) {
  return (
    <div className={`
      relative overflow-hidden rounded-xl p-6 
      ${gradient 
        ? 'bg-gradient-to-br from-dark-900/90 to-dark-950/95' 
        : 'bg-dark-900/80'
      }
      border border-white/10 
      shadow-lg shadow-black/30 
      backdrop-blur-xl
      ${hover ? 'hover:border-primary-400/30 hover:shadow-2xl hover:shadow-primary-500/20 hover:-translate-y-1 transition-all duration-300' : ''}
      ${className}
    `}>
      {gradient && (
        <div className="absolute top-0 right-0 w-24 h-24 bg-gradient-radial from-primary-500/15 to-transparent pointer-events-none" />
      )}
      {children}
    </div>
  );
}
```

### Form Input Component (React)
```jsx
export function Input({ label, error, icon, ...props }) {
  return (
    <div className="space-y-2">
      {label && (
        <label className="block text-sm font-medium text-white/70">
          {label}
        </label>
      )}
      <div className="relative">
        {icon && (
          <div className="absolute left-4 top-1/2 -translate-y-1/2 text-white/40">
            {icon}
          </div>
        )}
        <input
          className={`
            w-full rounded-lg px-4 py-3 
            ${icon ? 'pl-12' : ''}
            bg-dark-900/50 border border-dark-700
            text-white placeholder:text-white/40
            focus:outline-none focus:border-accent-500 focus:ring-4 focus:ring-accent-500/10
            transition-all duration-300
            ${error ? 'border-danger focus:border-danger focus:ring-danger/10' : ''}
          `}
          {...props}
        />
      </div>
      {error && (
        <p className="text-sm text-danger">{error}</p>
      )}
    </div>
  );
}
```

### Modal Component (React)
```jsx
export function Modal({ isOpen, onClose, title, children }) {
  if (!isOpen) return null;
  
  return (
    <div 
      className="fixed inset-0 z-50 flex items-center justify-center bg-black/80 backdrop-blur-sm"
      onClick={onClose}
    >
      <div 
        className="
          bg-gradient-to-br from-dark-900/95 to-dark-950/98 
          border border-white/15 
          rounded-2xl p-8 max-w-lg w-full mx-4
          shadow-2xl shadow-black/50
          backdrop-blur-3xl
        "
        onClick={e => e.stopPropagation()}
      >
        <div className="flex items-center justify-between mb-6">
          <h2 className="text-2xl font-bold text-white">{title}</h2>
          <button 
            onClick={onClose}
            className="text-white/50 hover:text-white transition-colors"
          >
            ✕
          </button>
        </div>
        {children}
      </div>
    </div>
  );
}
```

### Table Row Component
```jsx
export function DataRow({ cells, onClick, highlight = false }) {
  return (
    <tr 
      onClick={onClick}
      className={`
        group cursor-pointer transition-all duration-200
        hover:bg-gradient-to-r hover:from-primary-500/10 hover:to-primary-500/5
        hover:shadow-[inset_0_0_0_1px_rgba(167,139,250,0.2)]
        hover:scale-[1.005]
        ${highlight ? 'bg-primary-500/5' : ''}
      `}
    >
      {cells.map((cell, i) => (
        <td key={i} className="px-4 py-4 border-b border-white/5">
          {cell}
        </td>
      ))}
    </tr>
  );
}
```

---

## 10. Asset Library

### Logo Files
```
📁 ~/dev/brand-assets/
├── talos-logo-icon.svg              # Crystal icon only
├── talos-logo-horizontal-white.svg  # Full logo with text (coming)
└── README.md                        # Usage guide
```

**Remote URLs (Production):**
- Icon: `https://talospro.ai/logos-final/talos-crystal-gradient.svg`
- Horizontal: `https://talospro.ai/logos-final/talos-logo-horizontal-white.svg`

### Icons
TalosPro uses **Lucide React** for consistent icon design:
```bash
npm install lucide-react
```

```jsx
import { Users, TrendingUp, Shield } from 'lucide-react';

<TrendingUp className="w-6 h-6 text-primary-400" />
```

**Icon Sizing:**
- Small: `w-4 h-4` (16px) - inline with text
- Medium: `w-6 h-6` (24px) - default UI icons
- Large: `w-8 h-8` (32px) - feature highlights
- Hero: `w-12 h-12` (48px) - marketing sections

### Color Variables (CSS Custom Properties)
```css
:root {
  /* Copy these into your project */
  --primary-500: #7c3aed;
  --primary-600: #6d28d9;
  --primary-700: #5b21b6;
  --primary-400: #a78bfa;
  --accent-500: #60a5fa;
  --accent-600: #3b82f6;
  --dark-950: #0d0d0f;
  --dark-900: #1a1a1f;
  --dark-800: #27272f;
  --dark-700: #34343f;
  --success: #10b981;
  --warning: #f59e0b;
  --danger: #ef4444;
}
```

### Screenshots (Good Examples)
```
📁 brand-assets/examples/
├── dashboard-hero.png       # Main dashboard view
├── table-hover.png          # Table interaction
├── card-elevation.png       # Card hover states
├── button-variants.png      # All button types
└── mobile-responsive.png    # Mobile layout
```
*(To be added by Pixel)*

---

## 11. Accessibility (a11y)

### Color Contrast
All text meets **WCAG AA** standards (4.5:1 for normal text, 3:1 for large text):
- White on #0d0d0f: ✅ 21:1 (AAA)
- White on #7c3aed: ✅ 4.6:1 (AA)
- #a78bfa on #0d0d0f: ✅ 8.5:1 (AAA)

### Interactive States
All interactive elements MUST have:
- **Default state** - visible and identifiable
- **Hover state** - clear visual feedback
- **Focus state** - keyboard navigation support
- **Active state** - press feedback

```css
/* Focus rings for keyboard navigation */
button:focus-visible {
  outline: 2px solid #60a5fa;
  outline-offset: 2px;
}
```

### Motion
Respect user preferences:
```css
@media (prefers-reduced-motion: reduce) {
  * {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
  }
}
```

---

## 12. Implementation Checklist

### For New Features/Pages
- [ ] Uses Inter font family
- [ ] Colors from approved palette only
- [ ] Proper heading hierarchy (H1 → H2 → H3)
- [ ] Mobile-first responsive design
- [ ] Hover states on all interactive elements
- [ ] Focus states for keyboard navigation
- [ ] Consistent spacing (multiples of 4px)
- [ ] Glassmorphism on elevated surfaces
- [ ] Proper logo usage (icon vs horizontal)
- [ ] Color contrast meets WCAG AA

### For Designers (Pixel)
- [ ] Design system variables configured in Figma
- [ ] Components match code implementation
- [ ] Spacing aligns with 4px grid
- [ ] Test designs in dark mode
- [ ] Export assets at 2x for retina displays
- [ ] Provide hover/active state designs

### For Developers
- [ ] Use Tailwind utility classes (avoid custom CSS)
- [ ] Reuse existing components (Button, Card, Input)
- [ ] Test on mobile + desktop breakpoints
- [ ] Add proper ARIA labels
- [ ] Optimize images (WebP, lazy loading)
- [ ] Check loading states (skeletons, spinners)

---

## 13. Brand Do's and Don'ts

### ✅ Do
- Use approved color combinations
- Maintain consistent spacing rhythm
- Apply glassmorphism to cards/panels
- Add subtle hover animations
- Keep designs clean and minimal
- Use purple for primary brand identity
- Test on dark backgrounds (our default)
- Prioritize readability over decoration

### ❌ Don't
- Introduce new colors without approval
- Use solid black backgrounds (#000000) - use #0d0d0f
- Over-animate - subtle is better
- Use bright neon colors
- Mix different design styles
- Use raster logos when SVG is available
- Add unnecessary gradients everywhere
- Compromise accessibility for aesthetics

---

## 14. Quick Reference

### Most Common Utility Classes
```html
<!-- Buttons -->
class="px-6 py-3 rounded-lg font-semibold transition-all duration-300"

<!-- Cards -->
class="p-6 bg-dark-900/80 border border-white/10 rounded-xl backdrop-blur-xl"

<!-- Text -->
class="text-white/87"      <!-- Body text -->
class="text-white/70"      <!-- Secondary text -->
class="text-white/50"      <!-- Muted text -->

<!-- Spacing -->
class="space-y-4"          <!-- Vertical stack, 16px gap -->
class="gap-6"              <!-- Grid/flex gap, 24px -->
class="mb-12"              <!-- Bottom margin, 48px -->

<!-- Gradients -->
class="bg-gradient-to-br from-primary-500 to-indigo-600"
class="bg-gradient-to-r from-primary-500/10 to-primary-500/5"
```

### Color Usage Quick Guide
| Need | Use |
|------|-----|
| Primary CTA | `bg-gradient-to-br from-primary-500 to-indigo-600` |
| Secondary CTA | `bg-white/5 border border-white/10` |
| Card background | `bg-dark-900/80 backdrop-blur-xl` |
| Page background | `bg-dark-950` |
| Hover highlight | `bg-primary-500/10` |
| Success message | `bg-success/10 text-success border-success/20` |
| Danger message | `bg-danger/10 text-danger border-danger/20` |

---

## Questions?

**For design decisions:** Ask Sunny or Pixel  
**For implementation:** Check existing components in `/talos-admin` or `/talos-frontend`  
**For assets:** See `~/dev/brand-assets/`

**Last Updated:** January 29, 2025 by Raven  
**Version:** 1.0  
**Status:** ✅ Production Ready
