# Admin Dashboard

A modern, fully responsive admin dashboard built with CSS Grid layout, featuring project management, announcements, trending sections, and an intuitive sidebar navigation.
Made as a front-end learning project of CSS Grid, building admin panels, and creating dashboard interfaces using pure HTML and CSS.

## Live Demo

[View Live Demo](https://leandroesposito.github.io/top-admin-dashboard/)

## Features

### Layout & Design
- **CSS Grid Architecture** - Complex grid layout system for optimal content organization
- **Fully Responsive** - Adapts seamlessly for multiple desktop screen sizes
- **Modern Card Design** - Interactive project cards with hover effects
- **Custom Color Scheme** - Purple-themed accent colors with smooth transitions

### Navigation
- **Sidebar Menu** - Collapsible-style navigation with icon support
- **Hover Effects** - Interactive elements with smooth transitions
- **Quick Actions** - New, Upload, and Share buttons for project management

### Dashboard Components
- **Projects Grid** - Dynamic card grid displaying user projects
- **Announcements Panel** - Latest updates and notifications
- **Trending Section** - Popular users and their projects
- **Search Bar** - Global search functionality
- **User Profile** - Quick access to user settings and notifications

### Interactive Elements
- Card scaling effects on hover
- Button press animations
- Input field focus states
- Sidebar item hover highlighting
- Smooth color transitions

## Technologies Used

- **HTML5** - Semantic markup
- **CSS3** - Grid, Flexbox, Custom Properties
- **SVG Icons** - Scalable vector graphics for all icons

## Project Structure

```
admin-dashboard/
├── index.html              # Main dashboard HTML
├── style.css              # All styling and layouts
├── icons/                 # SVG icon files
└── images/               # Profile images    
```

## CSS Grid Layout Structure

The dashboard uses a sophisticated grid system:

```css
.body-wrapper {
    display: grid;
    grid-template-columns: 1fr 4fr;      /* Sidebar + Main content */
    grid-template-rows: min-content 1fr;  /* Header + Content */
}

.main-content {
    display: grid;
    grid-template-columns: 1fr 20rem;     /* Projects + Side panels */
    gap: 1rem;
}

.projects {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(20rem, 1fr));
    gap: 1rem;
}
```

### Grid Areas Breakdown:
- **Sidebar** - Spans full height (row 1-3)
- **Header** - Top right area with search and user info
- **Main Content** - Projects grid, announcements, trending
- **Footer** - Full-width attribution

## Color Scheme

| Variable | Color | Usage |
|----------|-------|-------|
| `--theme-accent-color` | hsl(273, 79%, 46%) | Sidebar, buttons, accents |
| `--theme-accent-color-light` | hsl(273, 79%, 60%) | Hover states |
| `--font-light-color` | rgb(60, 60, 60) | Card text content |
| Background (main) | rgb(226, 232, 240) | Main content area |
| Background (header) | azure | Header section |
| Card background | white | Project cards |

## Interactive Features

### Project Cards
- Hover effect: Scale (1.1) with border color change
- Border-left accent changes from orange to theme color
- Smooth transition (0.5s ease-in-out)
- Elevated z-index on hover

### Buttons
- Hover: Background color lightens
- Active: Scale down to 0.9
- Border radius: 2rem (pill-shaped)

### Sidebar Navigation
- Hover: Background highlight
- Icons: 2rem x 2rem with consistent spacing
- Active states: Visual feedback

### Form Inputs
- Focus: Theme-colored outline
- Background: Changes from grey to white
- Border radius: 1rem (rounded)

## Dashboard Sections

### 1. Projects Grid
- Dynamic card layout
- Project title and description
- Action icons (favorite, watch, fork)
- Border-left accent indicator

### 2. Announcements
- Latest site updates
- Community announcements
- Privacy policy updates
- Separators between items

### 3. Trending
- User avatars with profile images
- Usernames and project names
- Grid/flex hybrid layout

### 4. Header Area
- Search functionality
- Notification bell
- User profile with greeting
- Quick action buttons

## Screenshots

| Wide Desktop View | Tablet/Narrow Desktop View |
|--------------|--------------|
| <img src="https://github.com/leandroesposito/top-admin-dashboard/blob/main/screenshots/screenshot_wide.png" height="400" alt="Wide Desktop View"/> | <img src="https://github.com/leandroesposito/top-admin-dashboard/blob/main/screenshots/screenshot_narrow.png" height="400" alt="Tablet/Narrow Desktop View"/> |

## Key Features Showcase

### CSS Grid Mastery
- Complex nested grid layouts
- Auto-fit and minmax() for responsive cards
- Grid spanning across rows and columns
- Alignment and justification techniques

### Modern CSS Features
- Custom properties (CSS variables)
- Smooth transitions and transforms
- Hover effects with scaling
- Focus states for accessibility

### Component Architecture
- Reusable card components
- Modular icon system
- Consistent spacing and typography
- Semantic HTML structure

## Development Notes
- All SVGs are from open-source icon sets
- Profile images are placeholder assets
- No JavaScript required for core functionality (enhancements optional)

## Acknowledgments

- Icons by [SVG Repo](https://www.svgrepo.com/)
- Profile images from [Flaticon](https://www.flaticon.com/) - Animals icons created by Freepik
- CSS Grid inspiration from modern dashboard designs

## Learning Outcomes

This dashboard demonstrates:
- Advanced CSS Grid techniques
- Responsive design principles
- Modern UI/UX patterns
- Component-based styling
- Efficient use of CSS variables
- Smooth animations and transitions

