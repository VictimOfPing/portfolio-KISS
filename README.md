# KISS - Latin Tech House Events Platform

![React](https://img.shields.io/badge/React-19.1.1-61DAFB?logo=react&logoColor=111111)
![TypeScript](https://img.shields.io/badge/TypeScript-5.8-3178C6?logo=typescript&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-7.1-646CFF?logo=vite&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-3.4-06B6D4?logo=tailwindcss&logoColor=white)
![Framer Motion](https://img.shields.io/badge/Framer%20Motion-12.23-0055FF?logo=framer&logoColor=white)
![Vercel](https://img.shields.io/badge/Deploy-Vercel-000000?logo=vercel&logoColor=white)

KISS needed a dedicated digital presence beyond event flyers and social posts: a fast, mobile-first website that could present the brand, promote upcoming nights, archive past events, and support booking inquiries.
The result is a production-ready React single-page application for Italy's first Latin Tech House experience, deployed at [getyourkisstonight.com](https://www.getyourkisstonight.com/) with SEO metadata, animated interactions, and event-focused routing.

## Screenshot / Preview

<p align="center">
  <img src="public/logo.svg" alt="KISS Latin Tech House brand preview" width="220" />
</p>

No final production screenshot is committed in this repository yet. The current preview uses the shipped brand asset, while the gallery structure is already wired for real event photography.

## Tech Stack

<p>
  <img src="https://skillicons.dev/icons?i=react,ts,vite,tailwind,vercel" alt="React, TypeScript, Vite, Tailwind CSS and Vercel" />
</p>

- **Frontend:** React 19, TypeScript, React Router
- **Styling:** Tailwind CSS with a custom KISS design system, PP Monument Extended, Heebo, and Space Grotesk
- **Motion:** Framer Motion for preloader, page sections, parallax movement, hover states, and scroll-triggered reveals
- **SEO/PWA:** Static meta tags, Open Graph, JSON-LD organization schema, sitemap, robots file, manifest, and canonical URLs
- **Deployment:** Vite production build with Vercel SPA fallback routing

## Features

- Animated landing experience with a branded preloader, full-screen hero, parallax movement, and scroll-aware navigation.
- Event discovery flow for upcoming events, past event archive, venue details, artist lineups, and ticket/VIP call-to-actions.
- Responsive gallery layout with modal preview behavior and load-more pagination prepared for real event media.
- Dedicated contact route with booking copy, contact details, and an inquiry form wired with controlled React state.
- SEO-ready page foundation for a music/event brand, including structured data for KISS as an organization founded in Milan.

## Project Structure

The app is structured as a Vite React SPA with route-level pages and reusable brand sections:

```text
src/
  App.tsx                    # BrowserRouter setup and public routes
  pages/                     # Page-level compositions: Home, About, Events, Gallery, Contact
  components/                # Reusable UI sections and behavior
    HeroSection.tsx          # Brand-first landing section with motion
    UpcomingEvents.tsx       # Upcoming event cards and load-more state
    PastEvents.tsx           # Past event archive
    Gallery.tsx              # Responsive media grid and modal
    SEOHead.tsx              # Runtime metadata updates per page
  index.css                  # Tailwind layers, fonts, shared component classes
public/
  logo.svg / logo.png        # Brand assets
  manifest.json              # PWA metadata
  sitemap.xml / robots.txt   # Search indexing support
```

Routing is handled client-side with `react-router-dom`, while `vercel.json` rewrites clean URLs back to the SPA entry point so direct visits to `/about`, `/gallery`, or `/upcoming-events` resolve correctly in production.

## Results and Impact

- Launched a dedicated branded website for KISS at [www.getyourkisstonight.com](https://www.getyourkisstonight.com/).
- Turned the event brand into a searchable, shareable web property with canonical URLs, Open Graph tags, JSON-LD, sitemap, and PWA metadata.
- Created a scalable content structure for future event drops, past-event credibility, partner visibility, and booking inquiries.
- Preserved the club/event atmosphere through custom typography, a black-red visual system, motion-heavy interactions, and mobile-first layouts.

## Run Locally

```bash
npm install
npm run dev
```

Production build:

```bash
npm run build
```

## Contact

- **Live site:** [getyourkisstonight.com](https://www.getyourkisstonight.com/)
- **General inquiries:** info@getyourkisstonight.com
- **Bookings:** booking@getyourkisstonight.com
- **Portfolio case study:** [KISS live project](https://www.getyourkisstonight.com/)
