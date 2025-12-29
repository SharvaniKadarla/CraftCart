# CraftCart 🛒🎨  
*A DIY Learning & Craft Marketplace Platform*

CraftCart is a full-stack web application designed to bring together **DIY craft tutorials**, **product marketplaces**, and **creator studios** into a single, seamless platform. Users can explore step-by-step tutorials, watch instructional videos, shop for craft supplies, save favorites, manage carts, and creators can upload and manage their own content.

🔗 **Live Demo:** https://craftcart-seven.vercel.app/  

---

## 📌 Project Overview

CraftCart was developed as a **full-stack project** focusing on:
- Real-world e-commerce workflows
- Creator-driven tutorial content
- Modern web architecture using Next.js
- Scalable UI components and clean state management

The platform supports both **learners** and **creators**, blending education with commerce.

---

## ✨ Key Features

### 👤 Authentication & Users
- Secure user authentication (login, register, logout)
- User profiles with saved tutorials and wishlist
- Role-based access (general users & creators)

### 🛍️ Marketplace
- Browse craft products with images and details
- Product detail pages with dynamic routing
- Wishlist and cart functionality
- Checkout flow and order history

### 🎥 Tutorials & Videos
- Step-by-step craft tutorials
- Video-based learning with custom player
- Supplies list linked directly to marketplace items
- Save tutorials for later reference

### 🎨 Creator Studio
- Creator dashboard to upload tutorials and videos
- Studio editor with preview and step management
- Product linking for tutorial supplies

### ⚙️ Platform Capabilities
- Responsive design across devices
- Modular and reusable UI components
- Centralized data handling
- Clean separation of concerns (UI, data, logic)

---

## 🛠️ Tech Stack

### Frontend
- **Next.js (App Router)**
- **React**
- **JavaScript (ES6+)**
- **Tailwind CSS**
- **CSS Modules**

### Backend & Services
- **Supabase** (PostgreSQL database)
- **NextAuth.js** (Authentication)
- **Server Actions & Next.js API Routes**


### Tooling & Deployment
- **Vercel** (Hosting & CI/CD)
- **PostCSS**
- **ESLint**
- **GitHub**

---

## 🧱 Architecture Overview

CraftCart follows a **modular, scalable architecture** built on Next.js:

- **App Router (`src/app`)** for routing and layouts
- **Feature-based components** (cart, tutorial, studio, marketplace)
- **Centralized data sources** for products, tutorials, users, and videos
- **Reusable UI components** for consistency
- **Supabase client** for backend interaction

This structure ensures maintainability and scalability as features grow.

---
## 🖼️ Architecture Diagram

```text
Frontend (Next.js + Tailwind CSS)
        ↓
Backend API Routes (Next.js)
        ↓
Supabase (PostgreSQL)
        ↑
Authentication (NextAuth.js)
```

---
## 🔁 Component Interaction Flow

The platform follows a clear request–response lifecycle:
- User interacts with the frontend UI
- Frontend sends API requests to backend routes
- Backend validates session and applies business logic
- Data is fetched or updated in Supabase
- JSON response is returned to the frontend
- UI updates dynamically based on response

This ensures unidirectional data flow and consistent state updates.

---
## 🖼️ Component Interaction Diagram

``` text
User
 ↓
Frontend UI (Next.js)
 ↓  API Requests
Backend API Routes (Next.js)
 ↓        ↓
NextAuth  Supabase (PostgreSQL)
 ↑        ↑
Session   Data Response
Validated
 ↓
JSON Response
 ↓
Updated UI
```

---
## 🚀 Getting Started (Local Setup)

1️⃣ Clone the repository
- `git clone https://github.com/SharvaniKadarla/CraftCart.git`
- `cd CraftCart`

2️⃣ Install dependencies
- `npm install`

3️⃣ Run the development server
- `npm run dev`
- Open your browser at: `http://localhost:3000`

---
## 🌍 Deployment

CraftCart is deployed using **Vercel**.

🔗 **Live Application**:
https://craftcart-seven.vercel.app/

Deployment highlights:
- Automatic builds on push
- Optimized Next.js output
- Environment-based configuration

---
## 🔧 Key Implementations

- Dynamic routing for products, tutorials, and videos
- Secure authentication using NextAuth
- Supabase integration for data persistence
- Creator studio with live preview and step management
- Cart and wishlist state synchronization
- Modular, reusable UI components

This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.js`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
