# Luai Omer (Lasovar) – Portfolio

A single-page responsive portfolio built with HTML and CSS only (no JavaScript) for the Week 06 HCI Lab assignment.

- Live site: https://lasovar.github.io/luai.dev/
- Figma design: [Luai's Portfolio Mockup.fig](Luai's%20Portfolio%20Mockup.fig)

## Purpose and audience

The site presents my work as a game and engine programmer: my C++ engine **Quelos**, the games I've worked on, my skills, and how to contact me. It's aimed at game studios and recruiters, fellow developers, and the course assessors.

## Sections

Header, About, Projects, Skills, Contact, Footer.

## Design

- Colors: the [Dracula](https://draculatheme.com) palette (background `#282A36`, foreground `#F8F8F2`, purple `#BD93F9`, pink `#FF79C6`, plus cyan, green, orange, yellow, red and comment for accents)
- Fonts: Fira Code (headings, labels, code) and Inter (body text), from Google Fonts
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
