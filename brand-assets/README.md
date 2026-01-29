# 💎 TalosPro Brand Assets

This folder contains official TalosPro brand assets. Always use these approved files.

## Logo Files

### Icon Only (Crystal)
**File:** `talos-logo-icon.svg`  
**Use:** Favicons, app icons, social avatars, mobile headers  
**Sizes:** h-8 (32px), h-10 (40px), h-12 (48px)  
**Minimum:** 24px × 24px

### Horizontal Logo
**File:** `talos-logo-horizontal-white.svg` (to be added)  
**Use:** Desktop headers, marketing, email signatures  
**Sizes:** h-6 (24px), h-8 (32px), h-10 (40px)  
**Minimum:** h-6 (24px) / 0.75 inch

## Remote URLs (Production)

If you can't access these files directly:
```
Icon: https://talospro.ai/logos-final/talos-crystal-gradient.svg
Horizontal: https://talospro.ai/logos-final/talos-logo-horizontal-white.svg
```

## Usage Rules

✅ **Do:**
- Use SVG format (scales perfectly)
- Maintain aspect ratio
- Use on dark backgrounds (#0d0d0f preferred)
- Add backdrop if placing on photos: `bg-dark-950/80 backdrop-blur-md`

❌ **Don't:**
- Stretch or distort
- Change colors
- Add effects (shadows, outlines, etc.)
- Use on busy backgrounds without backdrop
- Recreate the logo

## Quick Implementation

### React/Next.js
```jsx
import Image from 'next/image';

// Icon only (mobile)
<Image 
  src="/logo.svg" 
  alt="TalosPro" 
  width={32} 
  height={32}
  className="h-8 w-8"
/>

// Responsive (icon mobile, horizontal desktop)
<div className="flex items-center gap-3">
  <Image src="/logo.svg" alt="TalosPro" width={32} height={32} className="h-8" />
  <span className="hidden sm:block text-xl font-bold">TalosPro</span>
</div>
```

### HTML
```html
<!-- Icon only -->
<img src="/logo.svg" alt="TalosPro" class="h-8">

<!-- Horizontal logo -->
<img src="/talos-logo-horizontal-white.svg" alt="TalosPro" class="h-6">
```

## Color Reference

The logo uses our brand gradients:
- **Purple to Coral:** `#8B5CF6 → #A855F7 → #F97316`
- **Highlight:** `#C4B5FD → #F9A8D4`
- **Shadow:** `#7C3AED → #9333EA`

See `BRAND_GUIDELINE.md` for full color palette.

## Need Help?

- **Full guidelines:** `~/dev/BRAND_GUIDELINE.md`
- **Questions:** Ask Sunny or Pixel
- **Issues:** Check if you're using correct file path

---

**Last Updated:** January 29, 2025  
**Maintained by:** Raven & Pixel
