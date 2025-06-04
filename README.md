# 🧱 Fullstack Starter Template

A scalable, production-ready fullstack starter template using:

- 🧑‍🎨 Frontend: [Next.js](https://nextjs.org/) + [TailwindCSS](https://tailwindcss.com/) + [ShadCN UI](https://ui.shadcn.com/) + [TypeScript](https://www.typescriptlang.org/)
- 🧠 Backend: [TypeScript](https://www.typescriptlang.org/) + [Express.js](https://expressjs.com/) + [PostgreSQL](https://www.postgresql.org/) + [Prisma ORM](https://www.prisma.io/)
- 🧹 Dev Tools: [ESLint](https://eslint.org/), [Prettier](https://prettier.io/), [Commitlint](https://commitlint.js.org/), [Husky](https://typicode.github.io/husky/), [Concurrently](https://www.npmjs.com/package/concurrently)

---

## 📁 Folder Structure

```

project-root/
│
├── frontend/                 # Next.js frontend
├── backend/                  # Express.js backend
│
├── .husky/                   # Git hooks via Husky
├── .github/                  # GitHub workflows / issue templates
│
├── commitlint.config.js      # Commit message rules
├── commit-lint.js            # Custom commit lint script
├── lint-all.js               # Lint frontend & backend together
│
├── LICENSE                   # MIT or your preferred license
├── README.md                 # This file
├── SECURITY.md               # Vulnerability reporting process
├── CONTRIBUTING.md           # Contribution guidelines
│
├── package.json              # Root-level scripts (e.g. dev, lint)
├── package-lock.json         # Lock file

````

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/rahil1202/FullStack-Next-Express-PostgreSQL-Template.git
cd fullstack-starter-template
````

### 2. Install Dependencies (root, frontend & backend)

```bash
npm install          # installs root + frontend + backend deps
# or if using separate commands:
npm install 
cd frontend && npm install  # installs  frontend deps
cd ../backend && npm install # installs  backend deps
```

Or use the root command if workspaces are configured.

---

## 🔄 Run the Project

You can run both frontend and backend from the **root folder** using:

```bash
npm run dev
```
This will start both servers concurrently in development mode.

If you want to run them separately, you can do so by navigating to each folder:
```bash
cd frontend && npm run dev  # starts Next.js frontend
cd ../backend && npm run dev # starts Express backend
```

This uses `concurrently` to run both servers:

* Frontend runs at: `http://localhost:3000`
* Backend runs at: `http://localhost:8080` (or configured port)

---

## 🔧 Available Scripts

### At root:

* `npm run dev` – Run both frontend and backend
* `npm run build` – Build both frontend and backend
* `npm run lint-all` – Lint all folders
* `npm run format-all` – Format with Prettier

### In `/frontend`

* `npm run dev` – Start Next.js dev server
* `npm run build` – Build frontend
* `npm run lint` – Lint frontend only
* `npm run format` – Format frontend only


### In `/backend`

* `npm run dev` – Start Express server with auto-restart
* `npm run build` – Build backend TypeScript code
* `npm run start` – Start built backend server
* `npm run lint` – Lint backend only
* `npm run format` – format backend only
* `npx prisma generate` – (Re)generate Prisma client
* `npx prisma migrate` – Run Prisma migrations

---

## ✅ Code Quality

* **ESLint + Prettier** – Linting and formatting
* **Husky + Commitlint** – Ensures all commits follow conventional format
* **lint-all.js** – Runs lint for both backend and frontend
* **format-all.js** – Runs prettier for both backend and frontend

---

## 🤝 Contributing

See [CONTRIBUTING.md](./CONTRIBUTING.md) for contribution guidelines.

---

## 🛡️ Security

If you find any security issue, please refer to [SECURITY.md](./SECURITY.md).

---

## 📄 License

This project is licensed under the [GNU License](./LICENSE).

---

## 🙌 Acknowledgements

* [ShadCN UI](https://ui.shadcn.com/)
* [Prisma](https://www.prisma.io/)
* [Husky](https://typicode.github.io/husky/)
* [Concurrently](https://www.npmjs.com/package/concurrently)
