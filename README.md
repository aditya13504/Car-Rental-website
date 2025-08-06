# CarRental-fullstack

## 🚗 Overview

CarRental-fullstack is a modern, full-stack web application for car rental services. It allows users to browse, book, and manage car rentals, while car owners can list and manage their vehicles and bookings. The project is built with React (frontend) and Node.js/Express (backend), using MongoDB for data storage.

---

## ✨ Features

- **User Features:**
  - Browse available cars with details and images
  - Book cars for specific dates and locations
  - View and manage your bookings
  - Responsive, modern UI with animations

- **Owner Features:**
  - Register as an owner and list cars
  - Manage car availability and details
  - View dashboard with stats (cars, bookings, revenue)
  - Manage bookings (approve/cancel)

---

## 🏗️ Technologies Used

- **Frontend:** React, Vite, TailwindCSS, react-router-dom, motion, axios
- **Backend:** Node.js, Express, MongoDB, Mongoose, JWT, bcrypt, multer, ImageKit
- **Other:** ESLint, Vercel (deployment), dotenv

---

## 📁 Folder Structure

```
CarRental-fullstack/
├── client/         # Frontend React app
│   ├── src/
│   │   ├── assets/         # Images and icons
│   │   ├── components/     # Reusable UI components
│   │   ├── context/        # React context for global state
│   │   ├── pages/          # App pages (Home, Cars, Bookings, Owner dashboard)
│   │   └── main.jsx        # App entry point
│   ├── public/             # Static files
│   ├── index.html          # Main HTML file
│   └── package.json        # Frontend dependencies
├── server/         # Backend Node.js app
│   ├── controllers/        # Route logic (user, owner, booking)
│   ├── models/             # Mongoose models (User, Car, Booking)
│   ├── routes/             # API routes
│   ├── configs/            # DB and ImageKit config
│   ├── middleware/         # Auth, file upload
│   ├── server.js           # Server entry point
│   └── package.json        # Backend dependencies
└── README.md       # Project documentation
```

---

## 🚀 Getting Started

### Prerequisites

- Node.js & npm
- MongoDB Atlas account (or local MongoDB)
- ImageKit account (for car image uploads)

### 1. Clone the Repository

```sh
git clone https://github.com/aditya13504/Car-Rental-website.git
cd CarRental-fullstack
```

### 2. Setup Backend

```sh
cd server
npm install
```

Create a `.env` file in `server/`:

```
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
IMAGEKIT_PUBLIC_KEY=your_imagekit_public_key
IMAGEKIT_PRIVATE_KEY=your_imagekit_private_key
IMAGEKIT_URL_ENDPOINT=your_imagekit_url_endpoint
```

Start the backend server:

```sh
npm run server
```

### 3. Setup Frontend

```sh
cd ../client
npm install
npm run dev
```

The frontend will run on [http://localhost:5173](http://localhost:5173) by default.

---

## 🧑‍💻 Usage Guide

1. **User:**
   - Register/login
   - Browse cars, view details, book cars
   - View/manage your bookings

2. **Owner:**
   - Change role to owner (from profile)
   - Add cars with images and details
   - View dashboard (stats, recent bookings, revenue)
   - Manage bookings (approve/cancel)

---

## 🛠️ API Endpoints (Backend)

- `/api/user/register` - Register user
- `/api/user/login` - Login user
- `/api/user/data` - Get user data
- `/api/user/cars` - Get all cars
- `/api/bookings/create` - Create booking
- `/api/bookings/user` - Get user bookings
- `/api/owner/change-role` - Become owner
- `/api/owner/add-car` - Add car
- `/api/owner/cars` - Get owner's cars
- `/api/owner/dashboard` - Owner dashboard data

---

## 📝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

---

## 📄 License

This project is licensed under the MIT License.

---

## 🙋 FAQ

**Q: Can I use this for my own car rental business?**
A: Yes! Feel free to fork and customize.

**Q: How do I deploy this?**
A: You can deploy the frontend on Vercel/Netlify and backend on Vercel/Render/Heroku. Update API URLs accordingly.

**Q: Where are images stored?**
A: Car images are uploaded to ImageKit for optimization and CDN delivery.

---

## 💡 Tips for Beginners

- Start by running the backend and frontend locally.
- Explore the UI and API endpoints using Postman or browser.
- Read the code in `client/src/pages` and `server/controllers` for logic.
- Don't hesitate to ask for help or search online for errors!