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

- Run npm create vite@latest my‑app -- --template react-ts and cd my‑app
- Install Tailwind dependencies: npm install tailwindcss @tailwindcss/vite
- Add tailwindcss to vite.config.ts:
```
import { defineConfig } from 'vite'
import tailwindcss from '@tailwindcss/vite'
export default defineConfig({
  plugins: [
    tailwindcss(),
  ],
})
```
- In src/index.css, add Tailwind import: 
```
@import "tailwindcss";
```
- Import index.css in src/main.tsx
- Create folder structure under src/: components/, pages/, assets/, styles/
- Add ESLint + Prettier: npm install -D eslint prettier eslint-config-prettier eslint-plugin-react and generate config files
- Add Husky pre‑commit hook for linting: npx husky-init && npm install
- Setup React Router: `npm install react-router-dom` and add basic `BrowserRouter` in `src/main.tsx`  
- Create a `Layout.tsx` in `components/` with `<Outlet/>` for nested routes  
- Add placeholder `LandingPage.tsx` in `pages/` and route at `/`
- Write README.md with “npm install” / “npm run dev” instructions
