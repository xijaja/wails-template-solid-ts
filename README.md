<p align="left">
<strong>English</strong> | 
<a href="https://github.com/xijaja/wails-template-solid-ts/blob/main/README_ZH.md">中文</a></p>
<h1 align="center">wails-template-solid-ts</h1>

<p align="center">Wails template which includes: Vite, Solid, TypeScript out of the box</p>

## Use this template

```bash
wails init -n my-wails-solid -t https://github.com/xijaja/wails-template-solid-ts
```

## Live Development

Run `wails dev` in the project directory to start it.

If you want to debug in the browser, please enter the `frontend` directory in another terminal, and then execute `npm run dev`, the front-end development server will run on http://localhost:34115.

## Tailwindcss

If you need to use tailwindcss and postcss, please enter the `frontend` directory,
Then run the command:

```bash
# isntall
npm install -D tailwindcss@latest postcss@latest autoprefixer@latest

# init tailwind.config.cjs and postcss.config.cjs
npx tailwindcss init tailwind.config.cjs -p
```

Create tailwind.css file and write:

```css
@import "tailwindcss/base";
@import "tailwindcss/components";
@import "tailwindcss/utilities";
```

Finally, import in `frontend/src/index.tsx`:

```tsx
import "./tailwind.css";
```

## Building

To build a redistributable, production mode package, use `wails build`.
