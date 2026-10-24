# Luai Omer (Lasovar) – Portfolio

A single-page responsive portfolio built with HTML and CSS only (no JavaScript) for the Week 06 HCI Lab assignment.

- Live site: https://luai.dev/
- Figma design: [Luai's Portfolio Mockup.fig](https://www.figma.com/design/7xsV1wVgkf86BUTdiOVADn/Dracula?node-id=0-1&t=cqREjTwWjAmnS3GY-1)

## Purpose and audience

The site presents my work as a game and engine programmer: **BANX**, the game I'm working on now, my C++ engine **Quelos**, the games I've worked on, my skills, and how to contact me. It's aimed at game studios and recruiters, fellow developers, and the course assessors.

## Sections

Header, Hero, BANX spotlight, About, Projects, Skills, Contact, Footer.

## Design

- Style: a comic-book / stylized game UI look inspired by Atlus menus (Persona 3 and 5, Metaphor: ReFantazio) and Hi-Fi Rush: thick ink outlines, hard offset shadows, halftone dots, sunbursts, skewed menu blocks, ransom-note lettering and slanted section edges
- Colors: taken from the BANX key art: balloon red `#E5202E`, lemon `#FFD83D`, sky `#6CC0F2`, ink `#121016` and paper `#FBF5E9`
- Fonts: Anton (headings), Bangers (comic sound effects), Archivo (body text and labels) and JetBrains Mono (code), from Google Fonts
- Icons: [Simple Icons](https://simpleicons.org), inlined as SVG

## Technical notes

- Semantic HTML5 (`header`, `nav`, `main`, `section`, `article`, `aside`, `footer`)
- Layout with Flexbox and the box model; sizes in `rem`, `em`, `%`, `vh` and `vw`
- Responsive breakpoints: tablet at 64em (1024px) and mobile at 40em (640px)
- Interactions without JavaScript:
  - Screenshot lightbox with `:target`
  - Roadmap accordion with `<details>`
  - Dismissible notice banner with the checkbox hack
  - Form validation with HTML attributes and `:valid` / `:invalid`
  - Scrolling ticker and beat-pulsing sticker with CSS animations (turned off for `prefers-reduced-motion`)
- HTML and CSS pass the W3C validators

## Structure

```
index.html    page content
style.css     all styles
images/       site assets (favicon)
README.md
```

Game cover art and screenshots load from their itch.io, Steam and GitHub pages.

## Running locally

Clone the repo and open `index.html` in a browser. No build step is needed.

## AI usage

Claude was used to help write the HTML and CSS from my Figma design and content, as allowed by the assignment's AI policy.
