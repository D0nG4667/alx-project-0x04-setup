# alx-project-0x04-setup

A **Next.js + TypeScript** project scaffold demonstrating best practices for building scalable applications with **shared layouts, Google Fonts integration, imperative routing, interface organization, custom error handling, and progressive state management patterns**.  

This repository is part of the **ALX Next.js learning series**, focusing on applying the **DRY principle**, clean architecture, and modern frontend development practices. It evolves across three linked projects:

- **alx-project-0x04** → Base setup with layouts, fonts, routing, interfaces, and custom error handling.  
- **alx-project-0x05** → Context API implementation for global state management.  
- **alx-project-0x06** → Redux Toolkit integration for complex, scalable state management.  

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
└── 📁alx-project-0x04-setup
    ├── 📁alx-project-0x04        # Base project
    ├── 📁alx-project-0x05        # Context API version
    └── 📁alx-project-0x06        # Redux Toolkit version
```

### alx-project-0x04 (Base Setup)

- **components/layouts** → Header, Footer, Layout  
- **components/common** → Button  
- **interface/index.ts** → Centralized TypeScript interfaces  
- **pages** → `_app.tsx`, `_document.tsx`, `index.tsx`, `404.tsx`, `counter-app.tsx`  
- **public** → Static assets (icons, SVGs)  
- **styles/globals.css** → TailwindCSS + Google Fonts  

### alx-project-0x05 (Context API)

- **context/CountContext.tsx** → Context provider and custom hook  
- **_app.tsx** → Wrapped with `UserProvider`  
- **counter-app.tsx** → Counter implemented with Context API  

### alx-project-0x06 (Redux Toolkit)

- **store/store.ts** → Redux store configuration  
- **slices** → Example slice for counter or user state  
- **_app.tsx** → Wrapped with Redux `Provider`  
- **counter-app.tsx** → Counter implemented with Redux hooks  

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

- Centralized `Header`, `Footer`, and `Layout` components.  
- Ensures **consistency** and adheres to the **DRY principle**.  

### 1. Google Fonts Integration  

- Imported **Montserrat** via `globals.css`.  
- Configured TailwindCSS to apply fonts globally.  

### 2. Imperative Routing  

- Landing page uses `useRouter` for **programmatic navigation**.  
- Buttons trigger route changes with explicit props.  

### 3. Interface Organization  

- All TypeScript interfaces extracted into `interface/index.ts`.  
- Promotes **clean architecture** and **type safety**.  

### 4. Custom 404 Page  

- Overridden default Next.js error page with a **styled 404.tsx**.  
- Includes navigation back to home with `react-icons/fa`.  

### 5. State Management Patterns  

- **useState**: Local component state for simple counters.  
- **Context API**: Global state with `CountContext` provider and custom hook.  
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

By working through this project series, you will:  

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
