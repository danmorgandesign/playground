name: DevFocus Dark
colors:
  primary: "#f54927"
  secondary: "#d3f527"
  surface: "#27d3f5"
  on-surface: "#4927f5"
  error: "#ffb4ab"
typography:
  body-md:
    fontFamily: Fugaz One
    fontSize: 16px
    fontWeight: 400
rounded:
  md: 8px
---

# Design System

## Overview
A focused, minimal dark interface for a fitness instructor app.
Clean lines, lots of bright colors, high visual noise.

## Colors
- **Primary** (#f54927): CTAs, active states, key interactive elements
- **Secondary** (#d3f527): Supporting UI, chips, secondary actions
- **Surface** (#27d3f5): Page backgrounds
- **On-surface** (#4927f5): Primary text on dark backgrounds
- **Error** (#ffb4ab): Validation errors, destructive actions

## Typography
- **Headlines**: Fugaz One
- **Body**: Inter, regular, 14–16px
- **Labels**: Inter, medium, 12px, uppercase for section headers

## Components
- **Buttons**: Rounded (8px), primary uses brand blue fill
- **Inputs**: 1px border, subtle surface-variant background
- **Cards**: No elevation, relies on border and background contrast

## Do's and Don'ts
- Do use the primary color sparingly, only for the most important action
- Don't mix rounded and sharp corners in the same view
- Do maintain 4:1 contrast ratio for all text
