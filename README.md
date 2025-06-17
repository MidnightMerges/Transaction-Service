# Transaction Service

A Node.js microservice for managing transactions, built with Express, TypeScript, and Sequelize ORM.

---

## 🚀 Features

-   Express REST API for transaction management
-   Sequelize ORM with MySQL support
-   TypeScript for type safety
-   Centralized error handling
-   Request tracing via Correlation IDs (AsyncLocalStorage)
-   Winston-based structured logging
-   Request validation with Zod

---

## 🛠️ Prerequisites

-   [Node.js](https://nodejs.org/)
-   [Git](https://git-scm.com/)
-   [MySQL](https://www.mysql.com/) (for database operations)

---

## 📦 Installation

```bash
# Clone the repository
git clone https://github.com/sidpd51/Node-Project-Template.git
cd Node-Project-Template

# Install dependencies
npm install

# Copy environment variables template and configure
cp .env.example .env
# Edit .env and set your environment variables (e.g., PORT)
```

---

## 🏃 Running the Service

### Development

```bash
npm run dev
```

### Production

```bash
npm run build
npm start
```

---

## 🧪 Project Structure

```
src/
  server.ts                # Entry point
  config/                  # Configuration files
  controllers/             # Express route handlers
  middlewares/             # Custom Express middlewares
  routers/                 # API route definitions
  utils/                   # Utility functions and error classes
  validators/              # Request validation logic
```

---

## 📝 API Endpoints

-   `GET /api/v1/bookings` – Retrieve bookings (sample endpoint)

---

## 🛡️ Error Handling

Centralized error handling using custom error classes in [`src/utils/errors/app.error.ts`](src/utils/errors/app.error.ts).

---

## 📖 Logging

Structured logging with Winston, including correlation IDs for tracing requests.

---

## 🧩 Extending

-   Add new routes in [`src/routers/v1`](src/routers/v1/index.ts)
-   Implement controllers in [`src/controllers`](src/controllers/bookingController.ts)
-   Add validation schemas in [`src/validators`](src/validators/index.ts)

---

## 📄 License

MIT

---
