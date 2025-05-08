---
description: Fully scaffold a React + Tailwind CSS app using Vite, ready for landing‑page development
alwaysApply: true
globs:
"*.js"
"*.jsx"
"*.ts"
"*.tsx"
---

When the user asks “scaffold React & Tailwind app with Vite”:

- [1 SP] Run npm create vite@latest my‑app -- --template react-ts and cd my‑app
- [1 SP] Install Tailwind dependencies: npm install -D tailwindcss postcss autoprefixer
- [1 SP] Run npx tailwindcss init -p to generate tailwind.config.cjs & postcss.config.cjs
- [1 SP] Configure tailwind.config.cjs with content: ["./index.html","./src/**/*.{js,ts,jsx,tsx}"]
- [1 SP] In src/index.css, add Tailwind directives (@tailwind base; @tailwind components; @tailwind utilities;)
- [1 SP] Import index.css in src/main.tsx
- [1 SP] Create folder structure under src/: components/, pages/, assets/, styles/
- [1 SP] Add ESLint + Prettier: npm install -D eslint prettier eslint-config-prettier eslint-plugin-react and generate config files
- [1 SP] Add Husky pre‑commit hook for linting: npx husky-init && npm install
- [1 SP] Create a LandingPage.tsx in pages/ with placeholder content
- [1 SP] Write README.md with “npm install” / “npm run dev” instructions
