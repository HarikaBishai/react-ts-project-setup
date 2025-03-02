# React Project Setup with Vite & Tailwind CSS

## 1. Create React Project - Named `registry`

📌 **Docs:** [Vite Guide](https://vite.dev/guide/)

### Command:

```sh
npm create vite@latest registry -- --template react-ts

```

## 2. Add tailwind

📌 **Docs:** [TailwindCSS Guide](https://tailwindcss.com/docs/installation/using-vite)

### Command:

```sh
npm install tailwindcss @tailwindcss/vite
```

## 3. Update the vite.config.js file to import and use the tailwindcss plugin

```js
import { defineConfig } from "vite";
import tailwindcss from "@tailwindcss/vite";

export default defineConfig({
  plugins: [tailwindcss()],
});
```

## 4. Import tailwind in src/index.css

```css
@import "tailwindcss";
```

## 5. Run the project

```sh
npm run dev
```
