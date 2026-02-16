# Light Gallery – Backend

**Light Gallery Backend** is a **Node.js + Express + MongoDB** backend powering the Light Gallery frontend.  
It provides secure **JWT authentication**, role-based access, product management, order handling, and user profile features.  
Designed to be **production-ready** with modular routes, controllers, and middleware.

🔗 **Live URL:**  
[https://light-gallery-backend-uosr.onrender.com/](https://light-gallery-backend-uosr.onrender.com/)

---

## Features

### 🔐 Authentication & Security
- JWT-based authentication with **Access Token + Refresh Token**
- Password reset via email/phone OTP
- Route protection via `verifyJWT` middleware
- Role-based access control (`authRoles`) for admin-only routes

### 👤 User Management
- Get current user profile
- Update user details
- Delete account
- Wishlist management
- Cart management (add, remove, clear, get products)
- Orders creation and viewing
- Email & phone verification

### 🛒 Product Management
- Add, update, delete products (admin only)
- Bulk product upload via CSV
- File uploads (images) handled via multer (disk/memory)
- Fetch products (admin / user / single product)

### 📝 Orders
- Create orders (user)
- Fetch orders (admin)

### 💳 Payments
- Cash on Delivery supported
- Online payment structure ready via Razorpay (integration pending)

---

## Tech Stack

**Backend**
- Node.js
- Express.js
- MongoDB + Mongoose
- JWT for authentication
- Cookie-parser
- CORS handling
- dotenv for environment variables

**Utilities**
- bcrypt for password hashing
- multer for file uploads
- csv-parser for bulk CSV products
- otp-generator for OTP verification
- Razorpay SDK (edge ready)
- Cloudinary for image storage
- Resend for email handling

---

## Project Structure (Simplified)

