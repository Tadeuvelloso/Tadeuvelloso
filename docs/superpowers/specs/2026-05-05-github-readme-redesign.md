# GitHub Profile README Redesign

**Date:** 2026-05-05  
**Goal:** Replace the current minimal README with a recruiter-focused profile that communicates skills, experience, and availability clearly.

## Context

- Target roles: Fullstack (React + Node/Express) and Frontend (React, Next.js)
- Experience: 3+ years
- Location: Florianópolis, Brasil
- Contact: LinkedIn + email (tadeuvellososilva@gmail.com)
- No featured projects (lost access to main project)

## Visual Style

Structured & Informative — adaptive light/dark theme matching the visitor's GitHub preference. Uses `prefers-color-scheme` via GitHub's native Picture element where needed, and theme-compatible services (github-readme-stats transparent theme).

## Sections

### 1. Header / Hero

- Animated typing SVG (readme-typing-svg) cycling: "Fullstack Developer", "React Developer", "Frontend Engineer"
- One-line bio: location · 3+ anos de experiência · Open to opportunities ✅
- LinkedIn badge + email badge visible above the fold

### 2. Tech Stack

Five categories with devicons (height=30, labels below):

| Category | Technologies |
|---|---|
| 🎨 Frontend | JavaScript, TypeScript, React, Next.js, HTML5, CSS3 |
| ⚙️ Backend | Node.js, Express, NestJS, GraphQL, Prisma |
| 🧪 Testes | Jest, Vitest, Playwright |
| 🗄️ Banco de Dados | PostgreSQL, MongoDB |
| 🛠️ Ferramentas | Git, GitHub, Slack |

Icons without devicon entries (none in final list) use shields.io badges.

### 3. GitHub Stats

Three cards side by side using external services, all with transparent/adaptive theme:

- **github-readme-stats** (anuraghazra) — general stats card
- **github-readme-streak-stats** (DenverCoder1) — contribution streak
- **github-readme-stats** top-langs — most used languages

### 4. Contact

- Section title: "Vamos conversar?" / "Let's talk?"
- Short invite sentence
- LinkedIn clickable badge
- Email clickable badge
- Footer line: "Florianópolis, Brasil 🇧🇷 · Disponível para trabalho remoto"

## Implementation Notes

- Use `align="center"` on `<div>` wrappers for centering in GitHub Markdown
- Use `<picture>` + `<source media="(prefers-color-scheme: dark)">` for theme-adaptive images where needed
- Stats cards: append `&theme=transparent&hide_border=true` to URLs
- Typing SVG: use `https://readme-typing-svg.demolab.com` service
- User must replace LinkedIn URL placeholder before publishing
