# Agência Criativa Web

A modern, responsive digital agency website built as an educational project for the **Front-end Development course at EBAC (Responsive Websites module)**. The goal is to practice advanced layout techniques, interactive components, and clean front-end architecture.

---

## About This Project

This project started as a class assignment and was expanded to explore more advanced front-end concepts than the original brief required.  
The focus is to simulate a real digital agency website with:

- Clear information hierarchy
- Strong visual identity
- Interactive elements that feel professional and polished
- Fully responsive behavior across different screen sizes

The site is structured as a single-page experience with sections for hero, about, services, testimonials, and contact.

---

## Main Features

### Core Experience

- **Responsive Navigation**: Header with primary links and a clear call-to-action
- **Hero Section**: High-impact headline, supporting text and main CTA buttons
- **“Por Trás da Marca” (About) Section**: Grid highlighting leadership, team, and key case studies
- **“Como Podemos te Ajudar” (Services) Section**: Interactive services carousel with dynamic details
- **Testimonials**: Short quotes from fictional clients to reinforce credibility
- **Contact Section**: Contact details and a basic contact form

---

### UI & UX

- **Design System**  
  Centralized CSS variables for colors, typography, spacing and shadows, making it easier to maintain consistency.

- **Gradient-Driven Visual Style**  
  Animated gradients on buttons and service cards for a modern, premium look.

- **Fluid Layout**  
  Combination of Flexbox and CSS Grid to adapt content to different viewports without breaking the structure.

- **Micro-Interactions**  
  Smooth transitions on hover states, cards, and content changes in the services section to make the interface feel more “alive”.

---

### Interactive Components

- **Services Carousel**  
  A custom JavaScript carousel that:

  - Highlights the active service card
  - Adjusts opacity and scale of neighboring cards to create depth
  - Updates a detailed information panel with icon, description and bullet points for each service

- **Team Modals**  
  “+” buttons on team members open a modal with:

  - Photo, name and role
  - Short professional highlight text
  - Bullet points with skills and experience

- **Portfolio Modal**  
  A dedicated modal for the “Explore Portfolio” CTA, currently showing a “portfolio under construction” message and prepared for future expansion.

- **Service Modal**  
  A simple informational modal linked to the services section, ready to display more detailed case information in the future.

All interactive behavior is implemented with **vanilla JavaScript** (no external libraries).

---

### Responsiveness

- **Breakpoint-Driven Layout**  
  Main breakpoint around `900px` to adapt from desktop layout to tablet/mobile:

  - Header spacing and navigation adjusted for smaller screens
  - Hero text and buttons realigned for better readability on narrow viewports
  - Services section reflows so the carousel and details remain usable on mobile

- **Flexible Typography & Spacing**  
  Font sizes and spacing were planned using a scale based on `rem`, keeping the design readable in different resolutions.

---

## Technologies Used

- **HTML5** – Semantic structure with sections for hero, about, services, testimonials and contact
- **CSS3** –
  - CSS Variables (custom properties)
  - Flexbox and Grid for layout
  - Transitions and keyframe animations for gradients and content changes
  - Media Queries for responsive behavior
- **JavaScript (ES6+)** –
  - Modular logic separated into files (`script.js` and `solucoes.js`)
  - DOM manipulation and event handling
  - Dynamic content updates (carousel, modals, details panel)

---

## Project Structure

```bash
Agencia CriativaWeb/
├── index.html          # Main page
├── README.md           # Project documentation
├── CSS/
│   ├── reset.css       # Base style reset
│   └── styles.css      # Theme, layout and animations
├── JS/
│   ├── script.js       # Navigation, member modals and general interactions
│   └── solucoes.js     # Services carousel and service modal
└── Assets/
    ├── Icons/          # Service icons
    └── ...             # Images and logo
```

---

## Design & Architecture Decisions

### Separation of Responsibilities

- `script.js` handles:
  - Header / navigation behavior
  - Team (members) modal logic
  - Portfolio modal behavior
- `solucoes.js` handles:
  - Services carousel states and animations
  - Dynamic update of the services details panel
  - Service modal logic

This separation keeps the code easier to read and maintain, especially as the project grows.

---

### Styling & Layout

- **CSS Variables** for colors, typography and spacing to avoid repetition and improve consistency.
- **Reusable Components** such as primary buttons (`.bt-large`), secondary buttons (`.bt-small`) and cards.
- **Animated Gradients** used in key areas (hero CTA, services, detail card) to reinforce a cohesive visual language.

---

## License

This project is open source and available under the **MIT License**.
