# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript and enable type-aware lint rules. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.

Why use Vite with React?

Vite is a modern, fast build tool that replaces Create React App (CRA). CRA is outdated and bloated; Vite is lean, insanely fast (thanks to ESBuild + Rollup), and developer-friendly.

Key Benefits

⚡ Blazing fast dev server (instant hot reloads, no waiting for webpack).

📦 Optimized production builds (tree-shaking, code-splitting).

🛠️ TypeScript, JSX, CSS, PostCSS, Tailwind — all out of the box.

🔌 Huge ecosystem of plugins (similar to Rollup’s).

🌍 Framework-agnostic (not just React, also Vue, Svelte, etc.).

How to Set Up React + Vite

Run the init command:

npm create vite@latest my-app


Choose React or React + TypeScript.

Install dependencies:

cd my-app
npm install


Start dev server:

npm run dev

Project Structure (default)
my-app/
├─ index.html
├─ src/
│  ├─ App.jsx
│  ├─ main.jsx
│  └─ assets/
├─ package.json

Example main.jsx
import React from 'react'
import ReactDOM from 'react-dom/client'
import App from './App'
import './index.css'

ReactDOM.createRoot(document.getElementById('root')).render(
  <React.StrictMode>
    <App />
  </React.StrictMode>
)

When NOT to use Vite

If you’re in a big enterprise project locked into Webpack (though you can migrate).

If you need very exotic build configurations that only Webpack supports.

If your team is already invested in Next.js (which handles SSR, routing, API endpoints).
