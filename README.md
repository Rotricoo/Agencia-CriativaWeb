# Creative Web Agency

A modern, responsive digital agency website showcasing professional front-end development practices. Built as an educational project for the **Front-end Development course at EBAC**, this site demonstrates advanced layout techniques, interactive components, and clean CSS architecture using the **BEM methodology**.

---

## About This Project

This project started as a class assignment and was expanded to explore more advanced front-end concepts than the original brief required. It has been completely refactored using the **BEM (Block, Element, Modifier) methodology** for CSS architecture, ensuring maintainability and scalability.

The site is structured as a single-page experience with sections for hero, about, services, testimonials, and contact.

---

## Main Features

### CSS Architecture & BEM Refactoring

**All CSS has been refactored to follow BEM (Block, Element, Modifier) standards**, ensuring:

- ✅ **Consistency**: Predictable naming convention across all 127+ BEM classes
- ✅ **Scalability**: Easy to add new components without conflicts
- ✅ **Maintainability**: Clear structure makes code updates straightforward
- ✅ **Low Specificity**: Single-class selectors prevent CSS conflicts
- ✅ **Reusability**: Modular components can be easily reused

### Core Experience

- **Responsive Navigation**: Header with mobile hamburger menu
- **Hero Section**: High-impact headline with CTA buttons
- **Behind the Brand Section**: Team grid with interactive modals
- **Solutions Carousel**: Dynamic services with real-time details
- **Testimonials**: Client quotes with navigation
- **Contact Section**: Contact form and information

### Interactive Components

- **Services Carousel**: Custom JavaScript carousel with `.solutions__card--active` modifier
- **Team Member Modals**: Photo, role, and professional details
- **Portfolio Modal**: "Coming soon" placeholder for future expansion

---

### UI & UX

- **Design System**
  Centralized CSS variables for colors, typography, spacing and shadows, making it easier to maintain consistency across the entire site.

- **Gradient-Driven Visual Style**
  Animated gradients on buttons and service cards create a modern, premium aesthetic that captures attention.

- **Fluid Layout**
  Combination of Flexbox and CSS Grid to adapt content to different viewports without breaking the structure or user experience.

- **Micro-Interactions**
  Smooth transitions on hover states, cards, and content changes in the services section make the interface feel polished and responsive.

---

### Responsiveness

- **Breakpoint-Driven Layout**
  Main breakpoint around `900px` adapts the design from desktop to tablet/mobile:

  - Header spacing and navigation restructured for smaller screens
  - Hero text and buttons realigned for optimal readability on narrow viewports
  - Services section reflows seamlessly, keeping the carousel and details usable on all devices

- **Flexible Typography & Spacing**
  Font sizes and spacing are built on a modular `rem`-based scale, ensuring consistent readability across all screen sizes and resolutions.

---

## Technologies Used

- **HTML5** – Semantic markup with structured sections for hero, about, services, testimonials and contact
- **CSS3** –
  - **BEM Methodology** for organized, scalable CSS architecture
  - CSS Variables (custom properties) for maintainable theming
  - Flexbox and Grid for modern, responsive layouts
  - Transitions and keyframe animations for smooth gradients and content changes
  - Media Queries for mobile-first responsive design (breakpoints at 900px and 405px)
- **JavaScript (ES6+)** –
  - Modular code split into focused files (`script.js` and `solutions.js`)
  - Efficient DOM manipulation and event handling
  - Dynamic content updates (carousel states, modal management)

---

## Project Structure

```bash
Creative-Web-Agency/
├── index.html          # Main page
├── README.md           # Project documentation
├── CSS/
│   ├── reset.css       # CSS reset for consistent cross-browser styling
│   └── styles.css      # Complete theme using BEM methodology
├── JS/
│   ├── script.js       # Navigation, team modals and general interactions
│   └── solutions.js    # Services carousel and service modal logic
└── Assets/
    ├── Icons/          # Service and brand icons
    └── Images/         # Team photos and project showcases
```

---

## Design & Architecture Decisions

### BEM Naming Convention

All CSS classes follow the **BEM (Block, Element, Modifier)** pattern:

**Examples in this project:**

- `.site-header`, `.site-header__nav`, `.site-header--open`
- `.hero`, `.hero__title`, `.hero__logo--mobile`
- `.team`, `.team__card`, `.team__card-small`
- `.solutions`, `.solutions__card`, `.solutions__card--active`
- `.testimonials__div`, `.testimonials__div--active`
- `.btn`, `.btn--primary`, `.btn--lg`

### Separation of Responsibilities

- `script.js` handles:
  - Header / navigation behavior
  - Team (members) modal logic
  - Portfolio modal behavior
- `solutions.js` handles:
  - Services carousel states and animations
  - Dynamic update of the services details panel
  - Service modal logic

This separation keeps the code easier to read and maintain, especially as the project grows.

---

## CSS Architecture Metrics

| Metric                  | Value            |
| ----------------------- | ---------------- |
| **Total CSS Lines**     | 1,381            |
| **BEM Classes**         | 127+             |
| **CSS Variables**       | 23               |
| **Breakpoints**         | 2 (900px, 405px) |
| **Average Specificity** | (0,1,0) - Low    |

---

## Learning Outcomes

This project demonstrates:

- **BEM CSS Methodology** for scalable, maintainable stylesheets
- **Responsive Web Design** with mobile-first approach
- **CSS Variables** for dynamic theming
- **CSS Grid & Flexbox** for modern layouts
- **JavaScript DOM Manipulation** without frameworks
- **Semantic HTML5** markup
- **Git & GitHub** workflow for version control

---

## License

This project is open source and available under the **MIT License**.
