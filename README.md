# alx-project-0x04-setup

A **Next.js + TypeScript** project scaffold demonstrating best practices for building scalable applications with **shared layouts, Google Fonts integration, imperative routing, interface organization, custom error handling, and progressive state management patterns**.  

This repository is part of the **ALX Next.js learning series**, focusing on applying the **DRY principle**, clean architecture, and modern frontend development practices.

---

## 🚀 Objectives

- Implement a **shared layout** (Header, Footer, Layout wrapper) across multiple pages.  
- Import and configure **Google Fonts** globally with TailwindCSS.  
- Set up a **landing page** with imperative routing using `useRouter`.  
- Organize and centralize **TypeScript interfaces** for maintainability.  
- Override Next.js’ default 404 with a **custom error page**.  
- Explore **state management approaches** (useState, Context API, Redux) in TypeScript for scalable applications.  

---

## 📂 Project Structure

```bash
└── 📁alx-project-0x04
    ├── 📁components
    │   ├── 📁common
    │   │   └── Button.tsx
    │   └── 📁layouts
    │       ├── Header.tsx
    │       ├── Footer.tsx
    │       └── Layout.tsx
    ├── 📁context
    │   └── UserContext.tsx        # Context API setup
    ├── 📁store
    │   ├── index.ts               # Redux store configuration
    │   ├── rootReducer.ts
    │   └── slices/
    │       └── userSlice.ts       # Redux slice example
    ├── 📁interface
    │   └── index.ts               # Centralized TypeScript interfaces
    ├── 📁pages
    │   ├── 📁api
    │   │   └── hello.ts
    │   ├── _app.tsx
    │   ├── _document.tsx
    │   ├── 404.tsx
    │   └── index.tsx
    ├── 📁public
    │   ├── favicon.ico
    │   ├── file.svg
    │   ├── globe.svg
    │   ├── next.svg
    │   ├── vercel.svg
    │   └── window.svg
    ├── 📁styles
    │   └── globals.css
    ├── .gitignore
    ├── eslint.config.mjs
    ├── next-env.d.ts
    ├── next.config.ts
    ├── package-lock.json
    ├── package.json
    ├── postcss.config.mjs
    ├── README.md
    └── tsconfig.json
```

---

## 🛠️ Setup Instructions

1. **Initialize the project**  

   ```bash
   npx create-next-app@latest alx-project-0x04
   cd alx-project-0x04
   ```

2. **Install dependencies**  

   ```bash
   npm install react-icons redux react-redux @reduxjs/toolkit @types/react-redux
   ```

3. **Run the development server**  

   ```bash
   npm run dev
   ```

   Visit [http://localhost:3000](http://localhost:3000) to preview changes.

---

## 📌 Implemented Features

### 0. Shared Layout  

- Centralized `Header`, `Footer`, and `Layout` components under `components/layouts`.  
- Ensures **consistency** and adheres to the **DRY principle**.  

### 1. Google Fonts Integration  

- Imported **Montserrat** via `styles/globals.css`.  
- Configured TailwindCSS to apply fonts globally.  

### 2. Imperative Routing  

- Landing page (`pages/index.tsx`) uses `useRouter` for **programmatic navigation**.  
- Buttons trigger route changes with explicit `pageRoute` props.  

### 3. Interface Organization  

- All TypeScript interfaces extracted into `interface/index.ts`.  
- Promotes **clean architecture** and **type safety**.  

### 4. Custom 404 Page  

- Overridden default Next.js error page with a **playful, styled 404.tsx**.  
- Includes navigation back to home with `react-icons/fa`.  

### 5. State Management Patterns  

- **useState**: Local component state for simple counters.  
- **Context API**: Global state with `UserContext` provider and custom hook.  
- **Redux Toolkit**: Centralized store with slices, typed hooks, and predictable state updates.  

---

## 🎨 Tech Stack

- **Next.js 15+** (Page Router ready)  
- **TypeScript** for type safety  
- **TailwindCSS** for utility-first styling  
- **React Icons** for scalable vector icons  
- **Redux Toolkit + Context API** for state management  

---

## 📖 Learning Outcomes

By working through this project, you will:  

- Understand **layout composition** in Next.js.  
- Learn how to **import and configure Google Fonts** with TailwindCSS.  
- Apply **imperative routing** using `useRouter`.  
- Organize **interfaces** for maintainability.  
- Customize **error handling** with a 404 page.  
- Compare **state management solutions** (useState, Context API, Redux) and know when to use each.  

---

## ✅ To Do

- Extend routing to additional mini‑apps.  
- Add dynamic data fetching with `getServerSideProps` or `getStaticProps`.  
- Explore **SEO optimization** with Next.js’ `<Head>` component.  
- Implement **middleware or persistence** for Redux state.  
- Optimize Context API with `React.memo` and `useMemo` to reduce re-renders.  
