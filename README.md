# Vite + React + TypeScript + PrimeReact DataTable

This project is a React application bootstrapped with **Vite** and written in **TypeScript**.  
It uses **PrimeReact DataTable** with **server-side pagination** and **persistent row selection**.

---

## 🚀 Features
- ⚡ Built with Vite + React + TypeScript
- 📊 PrimeReact DataTable
- 🔄 Server-side pagination (fetch new data on each page change)
- ✅ Row selection with checkboxes (single / multiple / select all)
- 🗂️ Custom selection panel
- ♻️ Selection persists across page changes
- 🌐 Deployable on Netlify / Cloudflare (not Vercel)

---

## 📦 Installation

1. Clone or extract the project:
   ```bash
   git clone <your-repo-url>
   cd vite-primereact-ts-datatable
   ```

   Or unzip the provided archive and `cd` into the folder.

2. Install dependencies:
   ```bash
   npm install
   ```

   ⚠ If you get an error with `primeicons@^8.0.0`,  
   change it to `^7.0.0` in `package.json`, then delete `node_modules` and `package-lock.json`, and run `npm install` again.

3. Run the development server:
   ```bash
   npm run dev
   ```

4. Open your browser at:
   ```
   http://localhost:5173
   ```

---

## 📂 Project Structure

```
vite-primereact-ts-datatable/
│── index.html
│── package.json
│── tsconfig.json
│── vite.config.ts
│
└── src/
    ├── main.tsx          # Entry point
    ├── App.tsx           # DataTable + pagination + selection
    ├── api.ts            # Mock API (replace with real backend)
    └── styles.css        # Global styles
```

---

## 🌐 Deployment (Netlify)

1. Push your code to GitHub.
2. Go to [Netlify](https://app.netlify.com/).
3. Connect your GitHub repo.
4. Set build command:
   ```
   npm run build
   ```
   And publish directory:
   ```
   dist
   ```
5. Deploy 🎉

---

## 📌 Notes
- Do **not** store all rows of all pages in memory.
- Always fetch fresh data from API on page change.
- Selection state is stored by row IDs and persists across pages.
