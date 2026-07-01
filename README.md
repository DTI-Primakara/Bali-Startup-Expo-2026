# 🚀 Bali Start-Up Expo 2026 (BSE 2026)

![BSE 2026 Logo](./src/assets/images/logo-bse-color.png)

**Ignite the Courage, Empower the Future**

Bali Start-Up Expo (BSE) 2026 is the largest innovation stage for local startups in Bali. As the pinnacle of technopreneur innovation from **Primakara University**, this platform connects dozens of selected digital startups with the community and industrial world.

---

## 📅 Event Details

| Detail | Information |
| :--- | :--- |
| **Date** | July 9 - 10, 2026 |
| **Venue** | [Discovery Mall Bali](https://maps.app.goo.gl/QFua9m7JCx8yQpxYA) |
| **Theme** | "From Small Step to Galaxy Innovation" |
| **Focus** | Digital Economy, Startup Innovation, Strategic Networking |

---

## ✨ Key Highlights

- **Startup Exhibition:** Showcasing brilliant ideas from 100+ booths.
- **Talkshows & Sharing Sessions:** Industry experts discussing Validation, Market Fit, and more.
- **Investor Pitching:** Connecting founders with potential strategic partners.
- **Competitions & Festivals:** MLBB Tournament, Coswalk Festival, and Startup Awards.
- **History of Impact:** A journey of innovation since 2015, empowering the Bali tech ecosystem.

---

## 🚀 Tech Stack

This project is built with a modern web development stack designed for high performance, modularity, and premium user experience:

- **Framework:** [Vue.js 3](https://vuejs.org/) (Composition API, `<script setup>` with TypeScript)
- **Language:** [TypeScript](https://www.typescriptlang.org/)
- **Styling:** [Tailwind CSS v4](https://tailwindcss.com/)
- **Animations:** [Motion-v](https://motion-v.com/) (Vue wrapper for Motion)
- **Build Tool:** [Vite 8](https://vite.dev/)
- **Linting & Formatting:** [oxfmt](https://github.com/oxc-project/oxc) for lightning-fast formatting.

---

## 📂 Project Structure

The project follows a modular, component-based directory layout:

```
├── .vscode/                 # Editor configuration settings
├── public/                  # Public assets (icons, images, etc.)
├── src/
│   ├── assets/              # Static assets, local logos, and media files
│   ├── components/          # Modular Vue components
│   │   ├── Header.vue       # Sticky navigation header with registration link
│   │   ├── HeroSection.vue  # Banner section with countdown timer & event info
│   │   ├── AboutSection.vue # Introduction to BSE, its mission, and background
│   │   ├── HistorySection.vue# Timeline detailing BSE's growth and impact since 2015
│   │   ├── HistoryBox.vue   # Helper component for history timeline nodes
│   │   ├── ActivitySection.vue# Talkshow and sharing session program details
│   │   ├── ActivityBox.vue   # Helper component displaying talkshow card details
│   │   ├── SideEventSection.vue# Special performances carousel interface
│   │   ├── SideEventBox.vue # Helper component for special performance cards
│   │   ├── WinnerSection.vue# Showcase of the BSE 2025 startup competition winners
│   │   ├── WinnerBox.vue    # Helper component for displaying winner details
│   │   ├── SponsorSection.vue# Showcase section for supporting partners
│   │   ├── MediaPartnerSection.vue# Infinite scrolling marquee for official media partners
│   │   ├── MediaPartnerBox.vue# Helper component for media partner logo cards
│   │   ├── GallerySection.vue# Gallery grid exhibiting highlights from previous years
│   │   ├── InvitationSection.vue# Interactive registration countdown and call-to-action
│   │   └── Footer.vue       # Footer containing navigation menus, social links, and organizer logos
│   ├── App.vue              # Main app entry layout coordinating all section renders
│   └── main.ts              # Entry script configuring dependencies
├── package.json             # Core dependency settings and CLI script triggers
├── vite.config.ts           # Configuration file for Vite build environment
└── tsconfig.json            # Base configuration for compiler options
```

---

## 🛠️ Getting Started

### Prerequisites

- **Node.js:** `^20.19.0` or `>=22.12.0`
- **Package Manager:** `npm` (included with Node.js)

### Installation

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd bse-2026
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Start the development server:**
   ```bash
   npm run dev
   ```

---

## 📜 Available Scripts

- **`npm run dev`**: Starts the Vite development server with external network access enabled (`--host`).
- **`npm run build`**: Runs TypeScript validation followed by bundling the application for production.
- **`npm run preview`**: Serves the generated production build locally for verification.
- **`npm run type-check`**: Validates project TypeScript files using `vue-tsc`.
- **`npm run format`**: Automatically formats the codebase utilizing the lightning-fast `oxfmt` formatter.

---

Built with ❤️ for the Bali Startup Ecosystem by the Primakara Community.
