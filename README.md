# SpendWise Dashboard Shell

A modern, responsive financial dashboard built with HTML and CSS, featuring CSS Grid and Flexbox layouts with a clean, professional design.

## Overview

This project implements the visual foundation for SpendWise, a personal finance management application. The dashboard displays spending categories with realistic static data and includes interactive hover effects and full responsive design.

## Features

### 1. Dashboard Layout
- **Sidebar Navigation**: Fixed left sidebar with navigation menu and branding
- **Header**: Top section with welcome message and action buttons
- **Category Cards**: Six financial category cards displaying spending data:
  - Food & Dining ($487.50)
  - Transport ($234.00)
  - Rent ($1,200.00)
  - Entertainment ($156.75)
  - Savings ($500.00)
  - Utilities ($189.30)

### 2. Modern CSS Techniques
- **CSS Grid**: Used for the main dashboard layout (sidebar + content area) and card grid
- **Flexbox**: Used for arranging header elements, sidebar navigation items, and content within each card
- **No absolute positioning**: Layout is entirely grid and flexbox based

### 3. Theme System (CSS Custom Properties)
The application uses CSS variables defined on the `:root` selector for consistent theming:
- `--brand-color`: Primary brand color (indigo)
- `--accent-color`: Accent color for positive trends (green)
- `--surface-color`: Card and surface backgrounds
- `--background-color`: Main page background
- `--text-primary`: Primary text color
- `--text-secondary`: Secondary text and labels

### 4. Responsive Design
- **Desktop**: Two-column layout with sidebar and main content
- **Mobile (< 768px)**: Single-column layout with horizontal scrolling navigation
- Tested using browser DevTools Device Toolbar

### 5. Micro-interactions
Cards feature smooth hover and focus animations:
- **Duration**: 200ms (under the 250ms requirement)
- **Effects**: Vertical lift (`translateY(-4px)`) and enhanced shadow
- **States**: Applied to both `:hover` and `:focus` for keyboard accessibility
- **Accessibility**: Cards have `tabindex="0"` for keyboard navigation

### 6. Dark Theme Support (Stretch Goal)
Automatic dark theme using `@media (prefers-color-scheme: dark)`:
- Overrides only CSS custom properties
- Adjusts colors for better contrast in dark mode
- Maintains all layout and functionality

## File Structure
