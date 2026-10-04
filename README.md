# IdeaDrop UI

A modern, responsive full-stack web application for sharing and managing ideas, featuring seamless user authentication, type-safe routing, and efficient server-state caching.

🔗 **Live Demo:** https://idea-drop-mu.vercel.app/  
🔗 **Backend API:** https://idea-drop-api-ryze.onrender.com  
Original Project by **[Brad Traversy](https://github.com/bradtraversy)**: [bradtraversy/idea-drop-ui](https://github.com/bradtraversy/idea-drop-ui)

---

## Learning Objectives

This project was developed as a hands-on learning project by following the **"Modern React From the Beginning"** course by [Brad Traversy](https://github.com/bradtraversy).  
The primary goal was to move from core React concepts to building a production-ready, full-stack client application with modern routing and data-fetching patterns.

Key concepts applied include:

* **Component-Based Architecture:** Structuring the UI into clean, reusable, and maintainable React components styled with Tailwind CSS.
* **Type-Safe File-Based Routing:** Implementing TanStack Router for route tree generation, layout routes, nested routing, and protected routes.
* **Server State Management:** Utilizing TanStack Query to manage query caching, background data refetching, mutations, and automatic cache invalidation.
* **Authentication & Authorization:** Implementing JWT-based authentication, user registration, login, automatic token refresh, and route guards.
* **Axios Interceptors:** Configuring request interceptors to automatically attach Bearer tokens and response interceptors to seamlessly handle 401 expiration and refresh token rotation.
* **CRUD API Integration:** Performing full CRUD (Create, Read, Update, Delete) operations on ideas by integrating with a REST API using Axios.
* **Context & Global State:** Managing authentication state across the application via React Context.
* **Environment Configuration:** Using `.env` files for securely configuring local and production API endpoints.
* **Modern Development Workflow:** Building with React 19, TypeScript, and Vite for optimal developer experience, fast build times, and deployment on Vercel.

---

## Features

- User registration and login
- JWT-based authentication with automatic token refresh
- Axios request & response interceptors for seamless Bearer token injection and 401 refresh handling
- Protected routes for authenticated actions (creating, editing, and deleting ideas)
- Complete CRUD operations for ideas
- Type-safe file-based routing with TanStack Router
- Efficient asynchronous state management with TanStack Query
- Dynamic route-based pages
- Clean, responsive UI built with Tailwind CSS v4 & Lucide React icons
- Environment-based configuration with `.env`
- Deployed-API friendly
- Frontend: React 19 + TypeScript (via Vite)
- Routing: TanStack Router
- State Management: TanStack Query
- Backend: IdeaDrop REST API (Node.js / Express / MongoDB)
- Communication: Axios (REST API)

---

## Application Routes

| Route | Page | Access | Description |
| :--- | :--- | :--- | :--- |
| `/` | Home | Public | Landing page featuring latest ideas and quick actions |
| `/ideas` | Ideas Explorer | Public | Browse all shared community ideas |
| `/ideas/$ideaId` | Idea Details | Public | View complete details, author info, and idea tags |
| `/ideas/new` | Create Idea | Protected | Form to create and submit a new idea |
| `/ideas/$ideaId/edit` | Edit Idea | Protected | Form to modify and update an existing idea |
| `/login` | Login | Public | User authentication page |
| `/register` | Register | Public | New account registration page |

---

## Original Creator & Credits

* **Original Creator:** [Brad Traversy](https://github.com/bradtraversy)
* **Original Repository:** [bradtraversy/idea-drop-ui](https://github.com/bradtraversy/idea-drop-ui)
* **API Repository:** [bradtraversy/idea-drop-api](https://github.com/bradtraversy/idea-drop-api)
* **Course:** Modern React From the Beginning

---

## Getting Started

### Prerequisites

Ensure you have Node.js (v18+) installed, and the [IdeaDrop API](https://github.com/bradtraversy/idea-drop-api) running locally or accessible remotely.

### Installation

1. Clone the repository and navigate to the UI directory:
   ```bash
   cd idea-drop-ui
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Configure environment variables in `.env`:
   ```env
   VITE_API_URL="http://localhost:5000"
   VITE_PRODUCTION_API_URL="https://idea-drop-api-ryze.onrender.com"
   ```

4. Available Scripts:
   - **Start dev server:**
     ```bash
     npm run dev
     ```
   - **Build for production:**
     ```bash
     npm run build
     ```
   - **Preview production build:**
     ```bash
     npm run preview
     ```
   - **Run tests:**
     ```bash
     npm test
     ```
   - **Run local mock JSON server:**
     ```bash
     npm run json-server
     ```

