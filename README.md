# Zerodha Clone

A Zerodha-inspired stock trading platform built as a learning project. The repository contains three separate apps:

- a public landing page for a brokerage brand
- a trading dashboard for holdings, positions, and watchlist data
- a backend API powered by Express and MongoDB for order and portfolio data

This project is meant to demonstrate how a real-world fintech UI can be structured across multiple frontend apps and a backend service.

## Overview

The project is split into three main parts:

1. `frontend/` – marketing website and user onboarding screens
2. `dashboard/` – trading dashboard UI with portfolio summary and watchlist
3. `backend/` – Node.js + Express API that stores data in MongoDB

## Tech Stack

### Frontend (landing page)
- React
- React Router
- Create React App

### Dashboard
- React
- React Router
- Material UI
- Chart.js and react-chartjs-2
- Axios

### Backend
- Node.js
- Express.js
- MongoDB
- Mongoose
- dotenv
- CORS

## Repository Structure

```text
Zerodha/
├── README.md
├── backend/
│   ├── .env
│   ├── index.js
│   ├── package.json
│   ├── package-lock.json
│   ├── model/
│   │   ├── HoldingsModel.js
│   │   ├── OrdersModel.js
│   │   └── PositionsModel.js
│   └── schemas/
│       ├── HoldingsSchema.js
│       ├── OrdersSchema.js
│       └── PositionsSchema.js
├── dashboard/
│   ├── package.json
│   ├── package-lock.json
│   ├── public/
│   └── src/
│       ├── components/
│       ├── data/
│       ├── index.css
│       └── index.js
├── frontend/
│   ├── package.json
│   ├── package-lock.json
│   ├── public/
│   ├── README.md
│   └── src/
│       ├── index.css
│       ├── index.js
│       └── landing_page/
│           ├── about/
│           ├── home/
│           ├── pricing/
│           ├── products/
│           ├── signup/
│           ├── support/
│           ├── Footer.js
│           ├── Navbar.js
│           ├── NotFound.js
│           └── OpenAccount.js
└── .gitignore