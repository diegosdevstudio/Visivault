# Contributing to VisiVault

Thank you for your interest in contributing to VisiVault! This document outlines the process for contributing to this DiegosDevStudio project.

-----

## 📋 Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Development Setup](#development-setup)
- [Coding Guidelines](#coding-guidelines)
- [Submitting a Pull Request](#submitting-a-pull-request)
- [Reporting Bugs](#reporting-bugs)
- [Suggesting Features](#suggesting-features)
- [Style Guidelines](#style-guidelines)

-----

## 🤝 Code of Conduct

By participating in this project you agree to:

- Be respectful and inclusive in all interactions
- Welcome constructive feedback graciously
- Focus on what’s best for the community and the project
- Show empathy towards other contributors

Harassment, discrimination, or abusive behavior of any kind will not be tolerated.

-----

## 💡 How Can I Contribute?

### Good First Issues

Look for issues tagged `good first issue` or `help wanted` in the GitHub issue tracker — these are ideal entry points for new contributors.

### Ways to Contribute

- 🐛 **Bug fixes** — Fix broken behavior and edge cases
- ✨ **Features** — Implement items from the roadmap or propose your own
- 📝 **Documentation** — Improve README, inline comments, or add examples
- 🎨 **Design** — Improve UI/UX, accessibility, or visual polish
- 🌐 **Translations** — Internationalize the UI
- 🧪 **Testing** — Add browser compatibility tests or prompt quality benchmarks

-----

## 🛠 Development Setup

```bash
# 1. Fork the repo on GitHub, then clone your fork
git clone https://github.com/YOUR_USERNAME/visivault.git
cd visivault

# 2. Create a feature branch
git checkout -b feat/your-feature-name

# 3. Open in browser
open index.html

# 4. Make your changes
# (No build step — edit index.html directly)

# 5. Test across browsers
# Chrome, Firefox, Safari, Edge
```

### Environment Variables / API Keys

Never commit API keys. The app loads the key from `localStorage` at runtime — no `.env` file is used or needed.

-----

## 📐 Coding Guidelines

### General

- Keep the project **single-file** (`index.html`) unless a feature genuinely warrants separation
- Prefer **vanilla JS** — no frameworks unless there’s a strong reason to add one
- All new JavaScript must be **ES2020+** compatible
- Keep CSS variables consistent with the existing design system (see `:root` block)

### Naming Conventions

|Type         |Convention    |Example         |
|-------------|--------------|----------------|
|CSS variables|`--kebab-case`|`--accent-color`|
|JS functions |`camelCase`   |`analyzeImage()`|
|JS constants |`UPPER_SNAKE` |`MAX_FILE_SIZE` |
|HTML IDs     |`camelCase`   |`visionOutput`  |
|CSS classes  |`kebab-case`  |`upload-zone`   |

### Security Rules

- **Never** log API keys to the console
- **Never** send the API key anywhere other than the intended Google API endpoint
- **Always** sanitize user-visible output with `escapeHtml()`
- **Always** display the Privacy & Consent Modal before any API call

### Accessibility

- Maintain `role`, `aria-label`, and `aria-selected` attributes on interactive elements
- Ensure keyboard navigability for all interactive components
- Maintain color contrast ratios of at least 4.5:1 for body text

-----

## 🔄 Submitting a Pull Request

1. **Sync with main** before opening your PR:
   
   ```bash
   git fetch upstream
   git rebase upstream/main
   ```
1. **Commit format** — use [Conventional Commits](https://www.conventionalcommits.org/):
   
   ```
   feat: add Midjourney aspect-ratio selector
   fix: correct base64 encoding for WEBP uploads
   docs: update API key setup instructions
   style: improve mobile tab layout
   refactor: extract API call to helper function
   ```
1. **PR Description** must include:
- What the PR does
- Why it’s needed
- Screenshots or screen recordings for UI changes
- Any breaking changes
1. **Review process:**
- A maintainer will review within 5 business days
- Address review feedback in new commits (don’t force-push during review)
- Once approved, a maintainer will squash-merge your PR

-----

## 🐛 Reporting Bugs

Open a GitHub Issue and include:

- **Browser & version** (e.g., Chrome 124, Safari 17)
- **Steps to reproduce** (numbered, minimal)
- **Expected behavior**
- **Actual behavior**
- **Console errors** (if any — screenshot or paste)
- **API response** (if API-related — redact your key!)

-----

## 🚀 Suggesting Features

Open a GitHub Issue with the `enhancement` label and describe:

- The problem you’re trying to solve
- Your proposed solution
- Any alternatives you considered
- Mockups or examples if applicable

**Roadmap ideas we’d love help with:**

- [ ] Midjourney `/imagine` formatted output mode
- [ ] Prompt history with localStorage
- [ ] Dark/Light theme toggle
- [ ] Export scenes as `.txt` or `.pdf`
- [ ] Multiple image batch analysis
- [ ] Claude API as an alternative backend

-----

## 🎨 Style Guidelines

VisiVault uses a **dark, refined editorial aesthetic**. When making UI changes:

- Typography: **Syne** (headings), **DM Mono** (body/code), **Fraunces** (accent/italic)
- Primary accent: `#6c63ff` (violet)
- Secondary accent: `#ff6584` (rose)
- Do not introduce new font families without discussion
- Maintain the noise texture and gradient mesh background system
- New UI elements should inherit from existing CSS variable tokens

-----

## 📄 License

By contributing to VisiVault, you agree that your contributions will be licensed under the [MIT License](LICENSE).

-----

<div align="center">

Thank you for making VisiVault better! — **DiegosDevStudio**

</div>
