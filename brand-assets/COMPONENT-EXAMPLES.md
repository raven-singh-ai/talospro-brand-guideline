# 🎨 TalosPro Component Examples

Quick copy-paste examples for common UI patterns. All use Tailwind + our design system.

---

## Buttons

### Primary Button (Main CTAs)
```jsx
<button className="
  px-6 py-3 rounded-lg font-semibold
  bg-gradient-to-br from-primary-500 to-indigo-600
  text-white
  shadow-lg shadow-primary-500/40
  hover:shadow-xl hover:shadow-primary-500/50
  hover:-translate-y-0.5
  active:translate-y-0
  transition-all duration-300
  relative overflow-hidden
  group
">
  <span className="relative z-10">Get Started</span>
  <span className="absolute inset-0 -left-full group-hover:left-full transition-all duration-500 bg-gradient-to-r from-transparent via-white/20 to-transparent" />
</button>
```

### Secondary Button
```jsx
<button className="
  px-6 py-3 rounded-lg font-semibold
  bg-white/5 border border-white/10
  text-white
  hover:bg-white/10 hover:border-white/20
  hover:-translate-y-0.5
  transition-all duration-300
">
  Learn More
</button>
```

### Ghost Button
```jsx
<button className="
  px-6 py-3 rounded-lg font-semibold
  bg-primary-500/5 border border-primary-500/20
  text-primary-300
  hover:bg-primary-500/15 hover:border-primary-400/40
  hover:shadow-lg hover:shadow-primary-500/30
  transition-all duration-300
">
  View Details
</button>
```

---

## Cards

### Standard Glass Card
```jsx
<div className="
  p-6 rounded-xl
  bg-gradient-to-br from-dark-900/90 to-dark-950/95
  border border-white/10
  backdrop-blur-xl
  shadow-lg shadow-black/30
  hover:border-primary-400/30
  hover:shadow-2xl hover:shadow-primary-500/20
  hover:-translate-y-1
  transition-all duration-300
">
  <h3 className="text-xl font-bold text-white mb-2">Card Title</h3>
  <p className="text-white/70">Card content goes here...</p>
</div>
```

### Stat Card with Gradient Accent
```jsx
<div className="
  relative overflow-hidden
  p-6 rounded-xl
  bg-dark-900/80
  border border-white/10
  backdrop-blur-xl
  hover:-translate-y-1
  transition-all duration-300
">
  {/* Gradient accent in corner */}
  <div className="absolute top-0 right-0 w-24 h-24 bg-gradient-radial from-primary-500/15 to-transparent pointer-events-none" />
  
  <div className="relative z-10">
    <p className="text-sm text-white/60 mb-1">Total Revenue</p>
    <p className="text-3xl font-bold text-white">$124,500</p>
    <p className="text-sm text-success mt-2">↑ 12.5% from last month</p>
  </div>
</div>
```

---

## Form Inputs

### Text Input
```jsx
<div className="space-y-2">
  <label className="block text-sm font-medium text-white/70">
    Email Address
  </label>
  <input
    type="email"
    placeholder="you@example.com"
    className="
      w-full px-4 py-3 rounded-lg
      bg-dark-900/50 border border-dark-700
      text-white placeholder:text-white/40
      focus:outline-none 
      focus:border-accent-500 
      focus:ring-4 focus:ring-accent-500/10
      transition-all duration-300
    "
  />
</div>
```

### Input with Icon
```jsx
<div className="relative">
  <div className="absolute left-4 top-1/2 -translate-y-1/2 text-white/40">
    <SearchIcon className="w-5 h-5" />
  </div>
  <input
    type="text"
    placeholder="Search..."
    className="
      w-full pl-12 pr-4 py-3 rounded-lg
      bg-dark-900/50 border border-dark-700
      text-white placeholder:text-white/40
      focus:outline-none 
      focus:border-accent-500 
      focus:ring-4 focus:ring-accent-500/10
      transition-all duration-300
    "
  />
</div>
```

### Input with Error State
```jsx
<div className="space-y-2">
  <input
    type="text"
    className="
      w-full px-4 py-3 rounded-lg
      bg-dark-900/50 border border-danger
      text-white placeholder:text-white/40
      focus:outline-none 
      focus:border-danger 
      focus:ring-4 focus:ring-danger/10
      transition-all duration-300
    "
  />
  <p className="text-sm text-danger">This field is required</p>
</div>
```

---

## Tables

### Modern Table with Hover
```jsx
<div className="overflow-x-auto rounded-xl border border-white/10">
  <table className="w-full">
    <thead>
      <tr className="bg-dark-800/50 border-b border-primary-500/20">
        <th className="px-6 py-4 text-left text-sm font-semibold text-white/70">
          Name
        </th>
        <th className="px-6 py-4 text-left text-sm font-semibold text-white/70">
          Status
        </th>
        <th className="px-6 py-4 text-left text-sm font-semibold text-white/70">
          Amount
        </th>
      </tr>
    </thead>
    <tbody>
      {data.map((row, i) => (
        <tr 
          key={i}
          className="
            border-b border-white/5
            hover:bg-gradient-to-r hover:from-primary-500/10 hover:to-primary-500/5
            hover:shadow-[inset_0_0_0_1px_rgba(167,139,250,0.2)]
            transition-all duration-200
            cursor-pointer
          "
        >
          <td className="px-6 py-4 text-white">{row.name}</td>
          <td className="px-6 py-4">
            <span className="px-3 py-1 rounded-full bg-success/10 text-success text-sm">
              {row.status}
            </span>
          </td>
          <td className="px-6 py-4 text-white">${row.amount}</td>
        </tr>
      ))}
    </tbody>
  </table>
</div>
```

---

## Modals

### Standard Modal
```jsx
{isOpen && (
  <div 
    className="fixed inset-0 z-50 flex items-center justify-center bg-black/80 backdrop-blur-sm"
    onClick={onClose}
  >
    <div 
      className="
        bg-gradient-to-br from-dark-900/95 to-dark-950/98
        border border-white/15
        rounded-2xl p-8
        max-w-lg w-full mx-4
        shadow-2xl shadow-black/50
        backdrop-blur-3xl
      "
      onClick={e => e.stopPropagation()}
    >
      {/* Header */}
      <div className="flex items-center justify-between mb-6">
        <h2 className="text-2xl font-bold text-white">Modal Title</h2>
        <button 
          onClick={onClose}
          className="text-white/50 hover:text-white transition-colors"
        >
          <XIcon className="w-6 h-6" />
        </button>
      </div>
      
      {/* Content */}
      <div className="space-y-4 mb-6">
        <p className="text-white/70">Modal content goes here...</p>
      </div>
      
      {/* Actions */}
      <div className="flex gap-3">
        <button className="flex-1 px-6 py-3 rounded-lg bg-white/5 border border-white/10 text-white hover:bg-white/10 transition-all">
          Cancel
        </button>
        <button className="flex-1 px-6 py-3 rounded-lg bg-gradient-to-br from-primary-500 to-indigo-600 text-white shadow-lg shadow-primary-500/40 hover:shadow-xl hover:-translate-y-0.5 transition-all">
          Confirm
        </button>
      </div>
    </div>
  </div>
)}
```

---

## Status Badges

### Success Badge
```jsx
<span className="
  inline-flex items-center gap-1.5
  px-3 py-1 rounded-full
  bg-success/10 text-success
  border border-success/20
  text-sm font-medium
">
  <CheckCircleIcon className="w-4 h-4" />
  Active
</span>
```

### Warning Badge
```jsx
<span className="
  inline-flex items-center gap-1.5
  px-3 py-1 rounded-full
  bg-warning/10 text-warning
  border border-warning/20
  text-sm font-medium
">
  <AlertCircleIcon className="w-4 h-4" />
  Pending
</span>
```

### Danger Badge
```jsx
<span className="
  inline-flex items-center gap-1.5
  px-3 py-1 rounded-full
  bg-danger/10 text-danger
  border border-danger/20
  text-sm font-medium
">
  <XCircleIcon className="w-4 h-4" />
  Failed
</span>
```

---

## Loading States

### Spinner
```jsx
<div className="flex items-center justify-center">
  <div className="
    w-8 h-8 rounded-full
    border-3 border-primary-500/20 border-t-primary-500
    animate-spin
  " />
</div>
```

### Skeleton Card
```jsx
<div className="
  p-6 rounded-xl
  bg-dark-900/80 border border-white/10
  backdrop-blur-xl
">
  {/* Title skeleton */}
  <div className="h-6 w-3/4 bg-gradient-to-r from-dark-700/40 via-dark-600/60 to-dark-700/40 rounded mb-3 animate-shimmer bg-[length:200%_100%]" />
  
  {/* Text skeleton */}
  <div className="h-4 w-full bg-gradient-to-r from-dark-700/40 via-dark-600/60 to-dark-700/40 rounded mb-2 animate-shimmer bg-[length:200%_100%]" />
  <div className="h-4 w-2/3 bg-gradient-to-r from-dark-700/40 via-dark-600/60 to-dark-700/40 rounded animate-shimmer bg-[length:200%_100%]" />
</div>

{/* Add to globals.css: */}
@keyframes shimmer {
  0% { background-position: -200% 0; }
  100% { background-position: 200% 0; }
}
```

---

## Gradient Text

```jsx
<h1 className="
  text-4xl font-bold
  bg-gradient-to-r from-primary-400 to-accent-500
  bg-clip-text text-transparent
">
  Welcome to TalosPro
</h1>
```

---

## Navigation Link (Sidebar)

```jsx
<a 
  href="/dashboard"
  className={`
    flex items-center gap-3 px-4 py-3 rounded-lg
    transition-all duration-300
    relative
    ${isActive 
      ? 'bg-primary-500/12 border-primary-400/25 shadow-[0_0_20px_rgba(124,58,237,0.15)]' 
      : 'border-transparent hover:bg-primary-500/15 hover:border-primary-400/30'
    }
    border
  `}
>
  {/* Active indicator */}
  {isActive && (
    <div className="absolute left-0 top-1/2 -translate-y-1/2 w-1 h-8 bg-gradient-to-b from-primary-400 to-primary-600 rounded-r" />
  )}
  
  <DashboardIcon className={`w-5 h-5 transition-all ${isActive ? 'text-primary-300 scale-110' : 'text-white/60'}`} />
  <span className={`font-medium ${isActive ? 'text-white' : 'text-white/70'}`}>
    Dashboard
  </span>
</a>
```

---

## Grid Layouts

### 3-Column Responsive Grid
```jsx
<div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
  {items.map(item => (
    <Card key={item.id}>{item.content}</Card>
  ))}
</div>
```

### Stats Grid (2-2-4 pattern)
```jsx
<div className="grid grid-cols-2 lg:grid-cols-4 gap-4">
  <StatCard title="Users" value="1,234" />
  <StatCard title="Revenue" value="$56K" />
  <StatCard title="Growth" value="+12%" />
  <StatCard title="Active" value="892" />
</div>
```

---

## Need More?

Check `BRAND_GUIDELINE.md` for:
- Complete design system
- Color palette
- Typography scale
- Accessibility guidelines
- Responsive patterns

**Pro tip:** All examples use Tailwind CSS. If a class doesn't exist, add it to your `tailwind.config.js` or `globals.css`.
