# Todo App - Fullstack

A fullstack Todo app built with NestJS (backend) and React (frontend). Node.js version used is v22.19.0.

<p align="center">
   <img src="https://raw.githubusercontent.com/ratukf/todo-frontend/refs/heads/master/src/assets/ui.png"/>
</p>

<p align="center">
   <img src="https://raw.githubusercontent.com/ratukf/todo-frontend/master/src/assets/ui2.png"/>
</p>

<p align="center">
   <img src="https://raw.githubusercontent.com/ratukf/todo-frontend/refs/heads/master/src/assets/ui3.png"/>
</p>

## Tech Stack

### Backend:

- **Node.js**
- **NestJS**
- **TypeScript**
- **TypeORM**
- **PostgreSQL / MySQL** (configurable)

### Frontend:

- **React js**
- **MUI**
- **React Query**
- **Axios**
- **Formik**
- **Yup**

## Features

- CRUD operations for Todo items
- Search Todos by title
- Patch Todo status and optional problem description
- DTO-based validation
- CORS enabled for frontend access

## Project Setup & Run

1. Clone the repository

```bash
git clone https://github.com/ratukf/todo

cd todo
```

2. Install dependencies

```bash
# Install todo dependencies

npm install
```

```bash
# Install todo-frontend dependencies

cd todo-frontend

npm install
```

```bash
# Install todo-backend dependencies

cd ../todo-backend

npm install
```

3. Setup environment

Copy `.env.example` to `.env` in the `todo-backend` folder:

```bash
cd todo-backend

cp .env.example .env
```

Edit each value inside `.env` file based on your PostgreSQL configuration & database (DB_HOST, DB_USER, DB_PASS, DB_NAME, etc).

4. Run the project

```bash
cd todo

# Run All (Backend & Frontend)
npm run start:all

# Run Backend
npm run start:backend

# Run Frontend
npm run start:frontend
```

## Technical Decision

1. **Modular Backend with NestJS & TypeORM:**
   Provides a clean and maintainable structure for entities, DTOs, and database migrations.
2. **React Query for Async State Management:**
   Efficiently handles CRUD operations with automatic cache invalidation, without the need for Redux.
3. **Formik + Yup for Form Handling & Validation:**
   Ensures consistent, reliable, and easy-to-validate forms in the frontend.

## License

MIT
