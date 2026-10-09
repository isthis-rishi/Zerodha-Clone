# 📈 Zerodha Clone — MERN Stack Trading Platform

A full-stack stock trading platform inspired by the interface and user experience of modern online brokerage websites. Built with the **MERN stack**—MongoDB, Express.js, React.js, and Node.js—this project demonstrates a separated frontend, trading dashboard, and backend REST API.

[![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)](https://www.mongodb.com/)
[![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)](https://expressjs.com/)
[![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)](https://react.dev/)
[![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org/)

> **Disclaimer:** This project is for educational purposes only. It is not affiliated with, endorsed by, or connected to Zerodha, and it does not support real financial transactions.

## 📝 About

This project recreates key elements of a modern brokerage platform as a learning application. It is organized into three parts:

- **Frontend:** A public-facing website with product information, pricing, support, and onboarding pages.
- **Dashboard:** A trading-style interface for viewing holdings, positions, orders, watchlists, and portfolio information.
- **Backend:** A Node.js and Express.js REST API that connects the dashboard to MongoDB using Mongoose.

The project demonstrates component-based React development, API communication, database modeling, and the separation of frontend and backend services.

## ✨ Features

### Public website
- Responsive landing page
- Home, About, Pricing, Products, and Support pages
- Signup and account-opening interface
- React Router navigation
- Reusable Navbar and Footer components
- Custom 404 page

### Trading dashboard
- Portfolio overview
- Holdings, positions, orders, and watchlist views
- Portfolio data visualization
- Axios-based API communication
- Material UI components
- Chart.js integration

### Backend API
- REST API built with Node.js and Express.js
- MongoDB integration with Mongoose
- Holdings, orders, and positions data management
- Environment variable configuration
- CORS configuration and database connectivity

## 🏗️ Architecture

```text
                 Client Applications
                         |
             +-----------+-----------+
             |                       |
             v                       v
      Public Frontend          Trading Dashboard
          React.js            React + Material UI
                                      |
                                  Axios / HTTP
                                      |
                                      v
                              Express REST API
                                Node.js
                                      |
                                  Mongoose
                                      |
                                      v
                                   MongoDB
```

## 🧰 Technology Stack

| Layer | Technologies |
|---|---|
| Frontend website | React.js, React Router |
| Trading dashboard | React.js, Material UI, Chart.js, Axios |
| Backend | Node.js, Express.js |
| Database | MongoDB, Mongoose |
| Communication | REST API, HTTP |
| Configuration | Environment variables |

## 📁 Project Structure

```text
.
├── backend/       # Node.js / Express API and database integration
├── dashboard/     # Trading dashboard built with React
├── frontend/      # Public-facing React website
└── README.md
```

## 🚀 Getting Started

### Prerequisites
- Node.js and npm
- MongoDB instance or MongoDB Atlas connection
- Git

### 1. Clone the repository

```bash
git clone https://github.com/isthis-rishi/Zerodha-Clone.git
cd Zerodha-Clone
```

### 2. Install dependencies

Install dependencies separately in each application directory that contains a `package.json`:

```bash
cd backend
npm install

cd ../frontend
npm install

cd ../dashboard
npm install
```

### 3. Configure environment variables

Create a `.env` file in the backend directory and add the environment variables expected by your backend code, such as your MongoDB connection string and server port. Check the source code for the exact variable names. Do not commit credentials or secret keys.

### 4. Run the applications

Open separate terminal windows for the backend, frontend, and dashboard. In each directory, run the script defined in its `package.json`, for example:

```bash
npm start
```

Some projects use `npm run dev` instead. Use the script configured in each application's `package.json`.

## 🔐 Development Notes

- Keep database credentials and other secrets in environment variables.
- Never commit `.env` files containing private credentials.
- Use sample or synthetic data for demonstrations.
- The project is a learning clone; do not use it to place real trades or handle real financial transactions.

## 🔭 Future Improvements

- Add authentication and role-based access, if required by the project scope.
- Improve validation and error handling for API requests.
- Add automated tests for frontend components and backend routes.
- Improve accessibility and responsive layouts.
- Connect to a market-data provider for a clearly labeled, non-trading demonstration, subject to provider terms.

## 🎓 Learning Outcomes

- Building React interfaces with reusable components
- Creating REST APIs with Node.js and Express.js
- Connecting an application to MongoDB using Mongoose
- Separating a full-stack project into independent services
- Fetching and visualizing data with Axios and Chart.js
- Managing environment-based configuration

## 🔎 Search Keywords

Zerodha clone, MERN stack project, stock trading dashboard, React trading UI, Node.js REST API, Express.js, MongoDB, Mongoose, portfolio dashboard, holdings management, orders management, positions dashboard, financial web application, full-stack web development.

## 🏷️ Suggested GitHub Topics

Add these topics individually in the repository's **About** section:

`zerodha-clone` `mern-stack` `mongodb` `expressjs` `react` `nodejs` `stock-trading` `trading-dashboard` `portfolio-management` `full-stack-development` `rest-api` `mongoose` `material-ui` `chartjs` `axios`

## 👤 Author

**Rishi Kumar**

GitHub: [@isthis-rishi](https://github.com/isthis-rishi)

## 📄 License

Add or retain a `LICENSE` file in the repository to clearly specify the terms under which others may use this project.

---

**Built as a full-stack learning project using the MERN stack.**
