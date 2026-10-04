# Zerodha Clone

A full-stack stock trading platform inspired by the interface and user experience of modern online brokerage platforms. This project was developed as a learning application to demonstrate the integration of React-based frontend applications with a Node.js/Express backend and MongoDB database.

> **Disclaimer:** This project is developed strictly for educational purposes. It is not affiliated with, endorsed by, or connected to Zerodha and does not support real financial transactions.

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Architecture](#architecture)
- [Technology Stack](#technology-stack)
- [Project Structure](#project-structure)
- [Database Design](#database-design)
- [API Architecture](#api-architecture)
- [Environment Configuration](#environment-configuration)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Running the Application](#running-the-application)
- [Screenshots](#screenshots)
- [Development Concepts](#development-concepts)
- [Future Improvements](#future-improvements)
- [Learning Outcomes](#learning-outcomes)
- [Author](#author)
- [License](#license)

---

## Overview

The Zerodha Clone is a full-stack web application divided into three independent applications:

1. **Frontend** – A public-facing brokerage website containing product information, pricing, support, and user onboarding pages.
2. **Dashboard** – A trading dashboard for displaying holdings, positions, orders, watchlist information, and portfolio data.
3. **Backend** – A REST API built with Node.js and Express.js that manages portfolio and order-related data stored in MongoDB.

The project demonstrates how different parts of a modern web application can be separated into independent frontend and backend services while communicating through REST APIs.

---

## Features

### Frontend

The frontend application provides the public-facing interface of the platform.

Features include:

- Responsive landing page
- Home page
- About page
- Pricing page
- Products page
- Support page
- Signup page
- Account-opening interface
- React Router navigation
- Reusable Navbar component
- Reusable Footer component
- Custom 404 Not Found page
- Component-based architecture

### Trading Dashboard

The dashboard represents the main trading interface.

Features include:

- Portfolio overview
- Holdings
- Positions
- Orders
- Watchlist
- Portfolio data visualization
- API-based data fetching
- Material UI components
- Chart.js integration
- Axios-based backend communication

### Backend

The backend provides the API layer between the dashboard and MongoDB.

Features include:

- Express.js REST API
- MongoDB integration
- Mongoose schemas and models
- Holdings management
- Orders management
- Positions management
- Environment variable configuration
- CORS configuration
- Database connectivity

---

## Architecture

The application follows a client-server architecture.

```text
                         Client Applications
                                |
                  +-------------+-------------+
                  |                           |
                  v                           v
           Frontend Application        Trading Dashboard
               React.js              React + Material UI
                                              |
                                              |
                                         HTTP / Axios
                                              |
                                              v
                                      Backend REST API
                                      Node.js + Express
                                              |
                                              |
                                           Mongoose
                                              |
                                              v
                                           MongoDB
