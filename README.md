# 🧛 Luai Salah (Lasovar): Personal Portfolio

## 📖 Project Overview

A **single-page responsive portfolio website** built with **HTML and CSS only (no JavaScript)** for the Week 06 HCI Lab assignment. It introduces me, my projects (my own C++ game engine, **Quelos**, and the games I've worked on), my skills, and how to contact me. The visual style follows the [Dracula](https://draculatheme.com) color theme.

- 🌐 **Live website:** https://lasovar.github.io/portfolio/ <!-- TODO: update if the repo name differs -->
- 🎨 **Figma design:** _add Figma link here_ <!-- TODO -->

## 🎯 Purpose

- Showcase my game engine work (Quelos) and the games I've contributed to, with links to play or wishlist them.
- Build a personal brand as a **game and engine programmer**, with a design that matches what I do: code-editor visuals and Dracula colors.
- Practice responsive layout with Flexbox, the box model, media queries and relative units.

## 👥 Target Audience

- **Game studios and recruiters** looking for a gameplay, engine or tools programmer.
- **Game jam teammates and other developers** who want to see my past jam games or talk about engines.
- **Lecturers and assessors** reviewing the lab assignment.

## 🧱 Technologies Used

- **HTML5** with semantic elements: `header`, `nav`, `main`, `section`, `article`, `aside`, `figure`, `footer`, `details`, `form`, `fieldset`
- **CSS3**: Flexbox, box model, custom properties (CSS variables), media queries, relative units (`rem`, `em`, `%`, `vh`, `vw`), transitions and keyframe animations
- **Google Fonts**: [Fira Code](https://fonts.google.com/specimen/Fira+Code) for headings, labels and code; [Inter](https://fonts.google.com/specimen/Inter) for body text
- **Icons**: brand logos from [Simple Icons](https://simpleicons.org), inlined as SVG
- **No JavaScript**: every interaction is done in HTML/CSS (see below)

## 📐 Layout & Sections

| # | Section | Contents |
| - | --- | --- |
| 1 | **Header** | Sticky bar with the `luai.dev` logo, in-page navigation and GitHub / itch.io / Steam icons |
| 2 | **Hero** | Name, tagline, call-to-action buttons and a code-editor window introducing me in C++ |
| 3 | **About me** | Profile card, short bio, what I care about as a developer, and a timeline |
| 4 | **Projects** | Featured Quelos engine card plus game cards for BANX, The Handbook and Catpire! with screenshot galleries |
| 5 | **Skills** | Icon tiles for core languages and tools (C++, C#, Rust, Odin, Python, Unity, Vulkan, JetBrains, …) plus grouped skill tags |
| 6 | **Contact** | Email, Discord, GitHub, itch.io and Steam, plus a contact form |
| 7 | **Footer** | Copyright, back-to-top link and social links |

## ✨ Interactive Features (pure CSS, no JavaScript)

| Feature | How it works |
| --- | --- |
| Screenshot lightbox | Clicking a thumbnail links to `#some-id`; the `:target` pseudo-class shows a full-screen overlay. The close button links back to the project. |
| Roadmap accordion | Native `<details>` / `<summary>`, with a rotating `+` icon styled using `[open]`. |
| Dismissible AI notice | Hidden checkbox + `<label>` close button; `.notice-toggle:checked + .notice { display: none; }` hides the banner. |
| Pill-style radio buttons | Visually hidden `<input type="radio">` + `:checked + label`. |
| Form validation | HTML attributes (`required`, `type="email"`, `minlength`) styled with `:valid` / `:invalid` once the user has typed (`:not(:placeholder-shown)`). |
| Blinking cursor | `@keyframes` animation on the hero title. |
| Hover effects | Cards lift, images zoom, icons change color, all using `transition`. |
| Smooth scrolling | `scroll-behavior: smooth` + `scroll-padding-top`, so the sticky header doesn't cover section titles. |
| Accessibility | Skip link, `:focus-visible` outlines, alt text on all images, ARIA labels on icon links, `prefers-reduced-motion` support. |

## 🎨 Design

The layout was sketched in Figma first and then built in code. Colors come from the official Dracula palette:

| Role | Name | Hex |
| --- | --- | --- |
| Page background | Background | `#282A36` |
| Cards / header | Darker background | `#21222C` |
| Borders, hover | Current Line / Selection | `#44475A` |
| Main text | Foreground | `#F8F8F2` |
| `// comments`, labels | Comment | `#6272A4` |
| Name highlight, hover | Pink | `#FF79C6` |
| Buttons, accents | Purple | `#BD93F9` |
| Links, types | Cyan | `#8BE9FD` |
| "Jam" badges, done items | Green | `#50FA7B` |
| "In development" badges | Orange | `#FFB86C` |
| Strings in code | Yellow | `#F1FA8C` |
| Invalid form input | Red | `#FF5555` |

## 📱 Responsiveness

Tested in browser dev tools at desktop, tablet and mobile widths.

| Breakpoint | Layout changes |
| --- | --- |
| **Desktop** (> 1024px) | Hero text and code window side by side; profile card sticks beside the bio; 3 game cards per row; 6 skill tiles per row |
| **Tablet** (≤ 64em / 1024px) | Hero, About, Quelos card and Contact stack vertically; game cards become horizontal rows; 4 skill tiles per row |
| **Mobile** (≤ 40em / 640px) | Navigation moves to its own scrollable row; cards stack vertically; form fields stack; 3 skill tiles per row; smaller code font |

## ✅ Validation

- HTML checked with the [W3C Markup Validation Service](https://validator.w3.org/): no errors.
- CSS checked with the [W3C CSS Validation Service](https://jigsaw.w3.org/css-validator/): no errors.

## 🧪 How to Run Locally

```bash
git clone https://github.com/Lasovar/portfolio.git
cd portfolio
```

Then open `index.html` in any browser (or use the VS Code **Live Server** extension). No build step is needed.

## 🚀 Deployment (GitHub Pages)

1. Push the repository to GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, then select `main` and `/ (root)`.
4. The site will be live at `https://lasovar.github.io/<repository-name>/`.

## 📂 Folder Structure

```
portfolio/
├── index.html      # The single page: header, hero, about, projects, skills, contact, footer
├── style.css       # All styles, organised into numbered sections
├── images/
│   └── favicon.svg # Site icon
└── README.md
```

Project cover art and screenshots are loaded from their official pages ([itch.io](https://luai-salah.itch.io/), [Steam](https://store.steampowered.com/app/3572810/BANX/) and the [Quelos repository](https://github.com/Lasovar/Quelos)), so they always match the live store pages.

## 📸 Screenshots

<!-- TODO: add screenshots, e.g. images/screenshot-desktop.png, -tablet.png, -mobile.png, and the Figma design -->

| Figma design | Desktop | Tablet | Mobile |
| --- | --- | --- | --- |
| _add_ | _add_ | _add_ | _add_ |

## 📄 Notes

- **AI usage:** Claude (Anthropic) was used to help write the HTML and CSS from my Figma design and content, as allowed by the assignment's AI policy.
- The contact form uses `mailto:`, so it opens the visitor's email app (static sites have no server to send mail).
