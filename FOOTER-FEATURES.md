# Footer Component Features

A modern, hacker-friendly footer that perfectly matches the onprem.in aesthetic.

## Design Highlights

### 🎨 Visual Elements
- **Terminal-style prompts** (`~/`, `$`, `#`) for section headers
- **Glowing green accents** (#44d62c) throughout
- **Pulsing status dot** showing "live" status
- **Animated hover states** on all links with arrow indicators
- **JetBrains Mono** for that authentic terminal feel
- **Subtle border glow** at top of footer

### 📋 Sections

#### 1. Brand Section
```
[onprem.in]
$ Your infrastructure. Your control.
● Building the future of on-premise
```
- Logo with bracket styling
- Tagline with terminal prompt
- Live status indicator with pulse animation

#### 2. Navigation Links
```
~/navigate
→ Home
→ Products
→ Solutions
→ Blog
```
- Quick access to main pages
- Hover reveals green arrows
- Terminal-style section headers

#### 3. Resources
```
$resources
→ Technical Guides
→ GitHub
→ Documentation
→ Support
```
- Links to helpful resources
- External links open in new tab

#### 4. Connect
```
#connect
→ hello@onprem.in
→ Twitter/X
→ LinkedIn
→ GitHub
```
- Social media links
- Email contact
- All external links properly configured

### 📧 Newsletter Section

**Terminal-style signup form:**
```
user@onprem.in:~/subscribe$
Stay in the loop
> your.email@company.com [subscribe ↗]
```

Features:
- Inline terminal prompt design
- Responsive layout (vertical on mobile)
- Green accent button with hover effects
- Animated submit icon
- Focus states with glow effect

### 📊 Footer Bottom Bar

```
© 2026 // onprem.in // Infrastructure Sovereignty
Privacy | Terms | build: v1.0.0
```

- Copyright with year
- Tagline: "Infrastructure Sovereignty"
- Privacy/Terms links
- Version/build info in terminal style
- All elements styled with green accents

## Interactions

### Link Hover States
- Color changes to green (#44d62c)
- Arrow indicators (`→`) fade in
- Slight transform movement
- Smooth transitions

### Newsletter Form
- Focus glow effect on input
- Button hover: lift + shadow
- Icon animation on hover
- Fully accessible with keyboard

### Responsive Behavior

**Desktop (> 1024px):**
- 4-column grid layout
- Newsletter in single row
- Bottom bar horizontal

**Tablet (640px - 1024px):**
- 2-column grid
- Brand spans full width

**Mobile (< 640px):**
- Single column stack
- Vertical newsletter form
- Centered bottom bar
- All text remains readable

## Technical Details

### Performance
- Pure CSS animations (no JS)
- Optimized hover states
- Minimal DOM elements
- Efficient grid layout

### Accessibility
- Semantic HTML
- Proper link rel attributes
- Keyboard navigable
- Screen reader friendly
- Form labels and placeholders

### Integration
- Automatically added to all pages via Layout.astro
- No manual imports needed per page
- Consistent across entire site

## Styling Philosophy

Matches the hacker-minimalist aesthetic:
- ✅ Terminal/command-line inspiration
- ✅ Green monochrome palette
- ✅ Monospace fonts for technical feel
- ✅ Subtle animations and microinteractions
- ✅ Professional yet approachable
- ✅ Clean, organized information hierarchy

## Customization

Easy to update:
- Social links in connect section
- Newsletter form action URL
- Build version in footer bottom
- Links and navigation items
- All styling via scoped CSS

---

**Location:** `/src/components/Footer.astro`
**Used in:** `/src/layouts/Layout.astro` (global)
**Appears on:** All pages automatically
