# 📋 Drag and Drop Todo Application

A lightweight, performant Task Management application built using React's functional component architecture and native browser Drag and Drop Web APIs.

## 🚀 Live Demo
Check out the production build running live on Netlify: 
👉 [Live Application Preview](https://netlify.com)

---

## 🛠️ Technical Stack & Tools
* **Core Library:** React.js (Functional Components)
* **State Management:** Native Hooks (`useState`, `useEffect`)
* **Browser API:** HTML5 Drag and Drop API
* **Deployment & CI/CD:** Netlify

---

## 🧠 Architectural Insights (For Mentees)

When reviewing this codebase, pay close attention to these architectural choices designed to mimic enterprise-grade frontend development:

### 1. Zero External Dependencies for UX
Instead of installing heavy drag-and-drop library wrappers (like `react-beautiful-dnd` or `dnd-kit`), this project utilizes native HTML5 event attributes (`draggable`, `onDragStart`, `onDragOver`, `onDrop`). This minimizes the bundle size and demonstrates deep mastery of core browser APIs.

### 2. Unidirectional Data Flow & State Updates
Task states are managed cleanly through immutable data updates. When a task card is moved across boards, index mappings change using pure functions, avoiding complex state mutations or synchronization bugs common in junior-level React apps.

### 3. Asynchronous Execution and Layout Independence
The components are decoupled. Column layouts dynamically calculate dropped coordinates independently from the rendering cycle of the child elements, keeping interactions fast and responsive.

---

## 💻 Getting Started Locally

Follow these quick steps to get the development environment running on your local machine:

1. **Clone the repository:**
   ```bash
   git clone

   ```

2. **Navigate into the project directory:**
   ```bash
   cd drag_and_drop_react_hooks
   ```

3. **Install dependencies:**
   ```bash
   npm install
   ```

4. **Launch the local development server:**
   ```bash
   npm run start
   ```
   Open [http://localhost:3000](http://localhost:3000) inside your web browser to interact with the application.

