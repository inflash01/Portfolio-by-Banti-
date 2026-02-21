# Portfolio Website Specification

## Project Overview
- **Project Name**: Banti Kumar Portfolio
- **Type**: High-end 3D Animated Portfolio Website
- **Core Functionality**: Showcase skills, projects, education, and contact information with immersive 3D visuals
- **Target Users**: Recruiters, potential clients, fellow developers

---

## UI/UX Specification

### Layout Structure

**Sections (Top to Bottom):**
1. **Navigation Bar** - Fixed, glassmorphism effect
2. **Hero Section** - Full viewport, 3D animated background
3. **About Me Section** - Two-column layout
4. **Projects Section** - 3D card grid
5. **Skills Section** - Animated progress bars
6. **Education Section** - Timeline layout
7. **Contact Section** - Form + social links
8. **Footer** - Minimal

**Responsive Breakpoints:**
- Mobile: < 768px
- Tablet: 768px - 1024px
- Desktop: > 1024px

### Visual Design

**Color Palette:**
- Background Primary: `#0a0a0f` (Deep black)
- Background Secondary: `#12121a` (Dark navy)
- Accent Primary: `#8b5cf6` (Violet)
- Accent Secondary: `#06b6d4` (Cyan)
- Accent Gradient: `linear-gradient(135deg, #8b5cf6 0%, #06b6d4 100%)`
- Text Primary: `#ffffff`
- Text Secondary: `#a1a1aa`
- Glass Background: `rgba(255, 255, 255, 0.05)`
- Glass Border: `rgba(255, 255, 255, 0.1)`

**Typography:**
- Headings: 'Clash Display', sans-serif (from CDN)
- Body: 'Satoshi', sans-serif (from CDN)
- Hero Name: 72px (desktop), 48px (mobile)
- Section Titles: 48px (desktop), 32px (mobile)
- Body Text: 16px
- Small Text: 14px

**Spacing System:**
- Section Padding: 100px vertical (desktop), 60px (mobile)
- Container Max Width: 1200px
- Card Padding: 32px
- Element Gap: 24px

**Visual Effects:**
- Glassmorphism: `backdrop-filter: blur(20px)`
- Card Glow: `box-shadow: 0 0 40px rgba(139, 92, 246, 0.3)`
- Text Glow: `text-shadow: 0 0 30px rgba(139, 92, 246, 0.5)`
- Smooth transitions: `transition: all 0.3s ease`

### Components

**1. Navigation Bar**
- Logo (left): "BK" with gradient
- Menu items (right): About, Projects, Skills, Contact
- Glassmorphism background
- Hover: text glow effect

**2. Hero Section**
- Full viewport height
- Three.js particle background
- Name: "Banti Kumar" with animated gradient text
- Subtitle: "B.Tech CSE (AIML) Student | Web Developer | Creative Designer"
- Typing effect for subtitle
- Two CTA buttons: "View Work" (gradient), "Contact Me" (outline)
- Scroll indicator at bottom

**3. About Me Section**
- Left: Circular profile image with glass border
- Right: Description text + quick stats (projects, experience, skills)
- Floating particles background

**4. Projects Section**
- 3D tilted card grid (2 columns desktop, 1 mobile)
- Cards: Whiteboard App (Python), Web Dev Projects, C++ Programs
- Hover: lift up + glow effect
- Modal on click

**5. Skills Section**
- Animated progress bars for: HTML, CSS, JavaScript, Python, C++
- Floating skill icons
- Percentage counters

**6. Education Section**
- Timeline layout
- Kashi Institute of Technology
- B.Tech CSE (AIML)
- ADCA & DCA Certified
- Animated entry on scroll

**7. Contact Section**
- Left: Contact form (name, email, message)
- Right: Social links (Instagram, YouTube, Email)
- Animated form with glow border
- Social icons with hover effects

**8. Footer**
- Copyright text
- Back to top button

---

## Functionality Specification

### Core Features

1. **Smooth Scroll Navigation** - Click nav items to scroll to sections
2. **3D Particle Background** - Interactive Three.js particles in hero
3. **Typing Animation** - Subtitle text types out automatically
4. **Scroll Animations** - GSAP-powered section reveals
5. **3D Project Cards** - Tilt effect on hover
6. **Animated Skill Bars** - Fill animation on scroll
7. **Modal Popup** - Project details in modal
8. **Form Validation** - Client-side form validation
9. **Responsive Design** - Mobile-first approach

### User Interactions
- Hover effects on all interactive elements
- Smooth scroll on nav click
- Card tilt on mouse move (projects)
- Button click animations
- Modal open/close

### Animations
- Page load: Staggered fade-in
- Scroll: Sections slide up with fade
- Hero: Particle movement + typing effect
- Skills: Progress bar fill animation
- Cards: 3D tilt on hover
- Buttons: Scale + glow on hover

---

## Technical Stack

- **Framework**: React + Vite
- **Styling**: Tailwind CSS
- **3D**: Three.js + @react-three/fiber + @react-three/drei
- **Animations**: GSAP + Framer Motion
- **Icons**: Lucide React
- **Fonts**: Google Fonts (Outfit, Space Grotesk)

---

## Acceptance Criteria

1. ✅ Page loads without errors
2. ✅ All sections visible and properly styled
3. ✅ Navigation smooth scrolls to sections
4. ✅ 3D particle background renders and animates
5. ✅ Typing animation works on hero subtitle
6. ✅ Project cards have 3D tilt effect
7. ✅ Skill bars animate on scroll
8. ✅ Contact form validates input
9. ✅ Fully responsive on mobile/tablet/desktop
10. ✅ No console errors
