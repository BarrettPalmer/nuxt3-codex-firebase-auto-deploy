# Website Build Prompt for Codex

Create a Nuxt 3 website using Tailwind CSS.

The site will have:

- A Home page at `/`
- An About Me page at `/about`

## Design

- Clean, modern layout
- Light background with dark text
- Use a centered container with max-width
- Add padding around content
- Use Google Fonts: 'Inter'

## Navigation

- Include a top navigation bar on all pages
- Nav bar should have:
  - Site title on the left ("MySite")
  - Links to "Home" and "About Me" on the right
  - Highlight current page link

## Home Page (`/`)

- Hero section with:
  - Large heading: "Welcome to MySite"
  - Subheading: "A simple Nuxt 3 website example"
  - Centered CTA button: "Learn More" → links to `/about`
- Below the hero:
  - 3-column grid with icons and text:
    - Fast
    - Simple
    - Open Source

## About Page (`/about`)

- Heading: "About Me"
- One paragraph of sample text
- Include a centered profile image (use placeholder URL)
- Add a contact email link below the bio

## Tailwind Setup

- Use Tailwind CSS via Nuxt module
- Add custom colors if needed
- Use utility classes for layout and spacing

## Components

- Create a reusable `Navbar.vue` component
- Use `Layout.vue` if needed for consistent nav across pages

## Project Structure

Let Codex decide the best file layout using Nuxt 3 defaults.

## End Result

A fully working Nuxt 3 project that runs with `npm run dev` and is ready for Firebase deployment.
