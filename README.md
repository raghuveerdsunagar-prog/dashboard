# Savra Teacher Insights Dashboard

A role-based **Admin Dashboard** for visualizing teacher activities such as lesson plans, quizzes, and question papers.  
Built with **React**, **Node.js/Express**, and **MySQL**, secured with **JWT authentication** and **bcrypt** password hashing.

---

## ✨ Features

- Admin-only access with secure login (JWT + bcrypt)
- Teacher summary cards (total lessons, quizzes, assessments, activities)
- Teacher selector to filter data per teacher
- Weekly trends line/bar chart for activities
- Activities distribution pie chart
- Protected API routes (only accessible with valid admin token)
- Logout and route guard for dashboard access

---

## 🛠 Tech Stack

**Frontend**
- React
- React Router
- Axios
- Chart library (e.g. Recharts / Chart.js – whichever you used)

**Backend**
- Node.js
- Express.js
- JWT (jsonwebtoken)
- bcrypt (for password hashing)
- MySQL (via a db connection module)

---

## 📂 Project Structure 

```bash
savradash/
├── backend/
│   ├── index.js          # Express server, routes, admin login, JWT middleware
│   ├── db.js             # MySQL connection
│   └── package.json
└── frontend/
    ├── src/
    │   ├── App.jsx
    │   ├── components/
    │   │   ├── Admin.jsx            # Admin login page
    │   │   ├── Dashboard.jsx        # Protected dashboard
    │   │   ├── Dashboardheader.jsx
    │   │   ├── Summary.jsx
    │   │   ├── TeacherSelector.jsx
    │   │   ├── Weeklycharts.jsx
    │   │   └── ActivitiesPie.jsx
    │   └── index.jsx
    └── package.json




# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) (or [oxc](https://oxc.rs) when used in [rolldown-vite](https://vite.dev/guide/rolldown)) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.
