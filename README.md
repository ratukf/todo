# Todo App - Fullstack

A minimal fullstack Todo app built with NestJS (backend) and React (frontend) built to fulfill a Full Stack technical test. **Node.js version used:** v22.19.0.

![Todo App Screenshot1](https://raw.githubusercontent.com/ratukf/todo-frontend/refs/heads/master/src/assets/ui.png)

![Todo App Screenshot2](https://raw.githubusercontent.com/ratukf/todo-frontend/master/src/assets/ui2.png)

![Todo App Screenshot3](https://raw.githubusercontent.com/ratukf/todo-frontend/refs/heads/master/src/assets/ui3.png)

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
cd todo-frontend

npm install
```

```bash
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
