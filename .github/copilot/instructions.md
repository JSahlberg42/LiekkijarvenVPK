# GitHub Copilot Instructions

## Project Context
This is a **basic-level school project** for the "Johdanto digitaalisiin palveluihin" (Introduction to Digital Services) course at Haaga-Helia.

## Project Overview
A simple website for **Liekkijärven VPK** (Volunteer Fire Department).

### Website Values
- **Luotettavuus** (Reliability)
- **Yhteisöllisyus** (Community)
- **Toiminnallisuus** (Functionality)

### Site Structure (3-5 pages):
- `index.html` - Home page (Etusivu) - Overview and highlights
- `toiminta.html` - Activities (Toiminta) - Detailed presentation of departments
- `liity.html` - Join us (Liity mukaan) - Membership criteria and recruitment
- `yhteystiedot.html` - Contact (Yhteystiedot) - Fire station address, key personnel and contact info
- All pages link to each other via mai

## Common Functionalities
- **Responsive navigation**: Mobile-first hamburger menu → expandable menu
- **Image lazy loading**: Use `loading="lazy"` attribute
- **Accessibility**: 
  - Sufficient contrast (AAA level)
  - Focus states (`:focus-visible`)
  - ARIA label attributes
  - Semantic tags
- **Language setting**: `lang="fi"`
- **CTA buttons**: Highlight color, clear texts ("Liity mukaan", "Ota yhteyttä")n menu
- Footer contains quick links and social media icons

### File Naming Conventions:
- **Images**: `vpk-hero.jpg`, `vpk-harjoitus-1.jpg`, `vpk-kalusto-1.jpg`, `vpk-nuoriso-1.jpg`, `logo-vpk.svg`
- **Icons**: `icon-phone.svg`, `icon-mail.svg`, `icon-location.svg`, `icon-calendar.svg`
- **CSS**: `styles.css`

## Tech Stack
- **Colors
- **Primary color**: Tumma laivastonsininen (Dark navy blue) #0F2A44 - header, dark text on light background
- **Highlight**: Pelastuspunainen (Emergency red) #C62828 - CTA buttons, important highlights
- **Secondary**: Vaalea harmaa (Light gray) #F5F7FA - background blocks
- **Text dark**: #1E2329
- **Text light**: #FFFFFF - light text on dark background
- **Link**: #0B72B9 (hover: #095A91)
- **Borders/dividers**: #D7DFE7

**CoFont families**:
  - **Headings**: Roboto Slab (clear, stable)
  - **Body text**: Inter (good readability on screens)
  - Loaded from Google Fonts

- **Heading levels**:
  - **H1**: 28–36px (mobile 28px, desktop 36px), bold
  - **H2**: 22–28px, semibold
  - **H3**: 18–22px, medium

- **Body text**: 16–18px, line-height 1.6–1.8
- **Links**: Clear color + underline on hover/focus, `:focus-visible` highlighting
- **Buttons**: 16–18px, large touch area (min 48x48px)
- **Accessibility**: Sufficient size and contrast, clear hierarchy, clear focus stateC62828, text #FFFFFF, hover darkens ~10%
- Links: clear color + underline on hover/focus, `:focus-visible` highlight
 (Mobile-First)
All layouts designed for mobile first, then adapted for larger screens.

- **Mobile (< 768px)**: 
  - Single column layout
  - Navigation Structure
- **Header**: Logo (links to index.html) in top bar
- **Mobile**: Hamburger → full-screen menu
- **Desktop**: Horizontal menu bar
- **Optional**: Breadcrumb trail (if multiple page levels are added)

### Components
- **Cards**: Use `.card`, `.card-header`, `.card-icon` classes
- **Buttons**: Use `.cta-button` class (min 48x48px touch targets)
- **Navigation**: Responsive navbar with hamburger menu on mobile
- **Images**: Add `loading="lazy"` for performance
- **Footer**: Quick links and social media icon links
- **Tablet (768px - 1023px)**: 
  - 2-column cards grid
  - More content visible
  - Content splits into two columns

- **Desktop (≥ 1024px)**: 
  - 1200px max width
  - 12-column grid system
  - 2-3 column divisions (cards 3-per-row)
  - Horizontal top navigation
  - Sticky header
  - Large showcase images
  - `--teksti-tumma` (#1E2329)
  - `--teksti-vaalea` (#FFFFFF)
  - `--linkki` (#0B72B9)
  - `--linkki-hover` (#095A91)
  - `--reunukset` (#D7DFE7)
### Language
- All content is in **Finnish**
- Use `lang="fi"` attribute

### Style
- **Color palette** defined in CSS variables:
  -Visual Theme
- **Style**: Clear, action-focused, illustrations from real VPK activities
- **Photography**: Real volunteer fire department activities
- Emphasize reliability, community, and functionality

## Important Notes
- Always include emergency number **112** in footer
- Keep content appropriate for a volunteer fire department
- Maintain consistent styling across all pages
- Images are in `/images/` folder
- Follow official naming conventions for new files
- All pages should link to each other via main navigation
- This is a **learning project** - keep suggestions beginner-friendly
- Focus on semantic HTML and accessibility best practices
### Typography
- **Headings**: Roboto Slab (serif)
- **Body**: Inter (sans-serif)
- Loaded from Google Fonts

### Responsive Design
- **Mobile-first** approach (< 768px)
- **Tablet** (768px - 1023px): 2-column cards grid
- **Desktop** (≥ 1024px): 3-column cards grid, sticky header

### Components
- **Cards**: Use `.card`, `.card-header`, `.card-icon` classes
- **Buttons**: Use `.cta-button` class (min 48x48px touch targets)
- **Navigation**: Responsive navbar with hamburger menu on mobile

## Code Style

### Keep it simple:
- Use basic HTML elements
- Use existing CSS classes from `styles.css`
- Follow the structure of existing pages
- Include proper alt text for images
- Maintain accessibility (ARIA labels, focus states)
- Add short HTML comments that explain element names and heading levels (e.g., h2 = level-2 heading)

### Common structure for all pages:
```html
<!DOCTYPE html>
<html lang="fi">
  <head>
    <!-- Meta tags, Google Fonts, stylesheet -->
  </head>
  <body>
    <header>
      <!-- Navigation + hero section -->
    </header>
    <main class="container">
      <!-- Page content -->
    </main>
    <footer>
      <!-- Copyright + emergency number 112 -->
    </footer>
  </body>
</html>
```

## Important Notes
- Always include emergency number **112** in footer
- Keep content appropriate for a volunteer fire department
- Maintain consistent styling across all pages
- Images are in `/images/` folder
- This is a **learning project** - keep suggestions beginner-friendly
