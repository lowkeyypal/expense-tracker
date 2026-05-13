<div align="center">

# Expense Tracker

**A full-stack MERN application for tracking income and expenses in real time**

[![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)](https://mongodb.com)
[![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)](https://expressjs.com)
[![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)](https://reactjs.org)
[![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](LICENSE)

</div>

---

## Overview

Expense Tracker is a full-stack web application built on the MERN stack that lets you log, categorize, and monitor your income and expenses. Transactions are persisted in MongoDB and the balance updates in real time as you add or remove entries.

---

## Features

- **Transaction Logging** — Add transactions with a description and amount
- **Income & Expense Split** — Separate views for money in and money out
- **Real-time Balance** — Total balance recalculates instantly on every change
- **Global State** — Managed with React Context API and a custom reducer
- **Persistent Storage** — All data stored and retrieved via MongoDB

---

## Tech Stack

<div align="center">

[![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)](https://mongodb.com)
[![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)](https://expressjs.com)
[![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)](https://reactjs.org)
[![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org)
[![Axios](https://img.shields.io/badge/Axios-5A29E4?style=for-the-badge&logo=axios&logoColor=white)](https://axios-http.com)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)

</div>

<br>

| Layer | Tools |
|---|---|
| **Frontend** | React, React Hooks, Context API |
| **Backend** | Node.js, Express.js |
| **Database** | MongoDB |
| **HTTP Client** | Axios |

---

## Project Structure

```
Expense-Tracker/
├── client/                         # React frontend
│   ├── public/
│   │   └── index.html
│   └── src/
│       ├── components/
│       │   ├── AddTransaction.js   # Form to add a new transaction
│       │   ├── Balance.js          # Displays current total balance
│       │   ├── Header.js           # App header
│       │   ├── IncomeExpenses.js   # Income vs expense summary
│       │   ├── Transaction.js      # Single transaction item
│       │   └── TransactionList.js  # Full list of transactions
│       ├── context/
│       │   ├── AppReducer.js       # State reducer logic
│       │   ├── GlobalContext.js    # Context definition
│       │   └── GlobalProvider.js   # Context provider wrapper
│       ├── utils/
│       │   └── format.js           # Currency formatting helpers
│       └── App.js
├── config/
│   ├── config.env                  # Environment variables
│   └── db.js                       # MongoDB connection
├── controllers/
│   └── transactions.js             # Route handler logic
├── models/
│   └── Transaction.js              # Mongoose transaction schema
├── routes/
│   └── transactions.js             # API route definitions
├── server.js                       # Express server entry point
└── package.json
```

---

## Getting Started

### Prerequisites

- Node.js 14+
- MongoDB instance *(local or Atlas)*
- npm

### Installation & Configuration

1. **Clone the repository**
   ```bash
   git clone https://github.com/silentwraith03/Expense-Tracker-MERN.git
   cd Expense-Tracker
   ```

2. **Install backend dependencies**
   ```bash
   npm install
   ```

3. **Install frontend dependencies**
   ```bash
   cd client
   npm install
   cd ..
   ```

4. **Configure environment variables**

   Create `config/config.env` and add the following:
   ```env
   MONGO_URI=your_mongodb_connection_string
   PORT=5000
   ```

---

## Usage

| Command | Description |
|---|---|
| `npm run dev` | Run frontend and backend concurrently |
| `npm run server` | Run backend only |
| `npm run client` | Run frontend only |
| `cd client && npm run build` | Build the frontend for production |

---

## Screenshots

<img src="images/sc1.png" width="32%"> <img src="images/sc2.png" width="32%"> <img src="images/sc3.png" width="32%">

---

## License

Distributed under the MIT License. See [`LICENSE`](LICENSE) for details.
