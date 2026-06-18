# Bali Start-Up Expo 2026 (BSE 2026)

![BSE 2026 Logo](./src/assets/images/logo-bse-color.png)

**Ignite the Courage, Empower the Future**

Bali Start-Up Expo (BSE) 2026 is the largest innovation stage for local startups in Bali. As the pinnacle of technopreneur innovation from **Primakara University**, this platform connects dozens of selected digital startups with the community and industrial world.

## 📅 Event Details
- **Date:** July 9 - 10, 2026
- **Venue:** Discovery Mall Bali
- **Theme:** "From Small Step to Galaxy Innovation"
- **Focus:** Digital Economy, Startup Innovation, Strategic Networking

## ✨ Key Highlights
- **Startup Exhibition:** Showcasing brilliant ideas from 100+ booths.
- **Talkshows & Sharing Sessions:** Industry experts discussing Validation, Market Fit, and more.
- **Investor Pitching:** Connecting founders with potential strategic partners.
- **Competitions:** MLBB Tournament, Coswalk Festival, and Startup Awards.
- **History of Impact:** A journey of innovation since 2015, empowering the Bali tech ecosystem.

## 🚀 Tech Stack

This project is built with a modern web development stack for high performance and a polished user experience:

- **Framework:** [Vue.js 3](https://vuejs.org/) (Composition API, `<script setup>`)
- **Language:** [TypeScript](https://www.typescriptlang.org/)
- **Styling:** [Tailwind CSS 4](https://tailwindcss.com/)
- **Animations:** [Motion-v](https://motion-v.com/) (Vue wrapper for Motion)
- **Build Tool:** [Vite 8](https://vitejs.dev/)
- **Linting & Formatting:** [oxfmt](https://github.com/oxc-project/oxc) for lightning-fast formatting.

## 📂 Project Structure

The project follows a modular component-based architecture:

- `src/components/`: Modular Vue components:
    - `HeroSection.vue`: Countdown timer and main event call-to-action.
    - `AboutSection.vue`: Introduction to BSE and its mission.
    - `HistorySection.vue`: Timeline of the event's growth since 2015.
    - `ActivitySection.vue`: Schedule of talkshows and sharing sessions.
    - `WinnerSection.vue`: Showcase of previous year's winners (BSE 2025).
    - `Sponsor & MediaPartner`: Branding for strategic collaborators.
- `src/assets/`: Static assets including images, logos, and custom fonts (Montserrat).
- `src/App.vue`: Root layout orchestrating all sections.
- `src/main.ts`: Application entry point.

## 🛠️ Getting Started

### Prerequisites

- **Node.js:** `^20.19.0` or `>=22.12.0`
- **Package Manager:** `npm` (included with Node.js)

### Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd bse-2026
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```

## 📜 Available Scripts

- `npm run dev`: Starts the Vite development server with host access.
- `npm run build`: Runs type-checking and builds the application for production.
- `npm run preview`: Previews the production build locally.
- `npm run type-check`: Runs `vue-tsc` to verify TypeScript types.
- `npm run format`: Formats the source code using `oxfmt`.

---

Built with ❤️ for the Bali Startup Ecosystem by the Primakara Community.
