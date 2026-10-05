# Zentro - Backend

The backend API for **Zentro**, a SaaS-based e-commerce and inventory management plaform

Zentro provides a marketplace where customers can browse products from approved vendors, while vendors manage their products, inventory, orders, and store status through their dashboard. Administrators manage vendors, approvals, categories, and platform-level operations.

##  Features

### Authentication & Authorization

- JWT-based authentication
- HTTP-only authentication cookies
- Role-based access control
- Customer registration and login
- Vendor registration with approval workflow
- Protected admin and vendor routes

### Admin Management

- Admin dashboard statistics
- Vendor management
- Vendor approval and rejection
- Vendor store status management
- Admin profile management
- Vendor approval notifications

### Vendor Management

- Vendor dashboard
- Product creation and management
- Product image uploads
- Inventory and stock management
- Minimum stock tracking
- Order management
- Approve or reject customer orders
- Sales and order statistics
- Vendor notifications

### Customer & Orders

- Public product browsing
- Product availability based on vendor approval and store status
- Cart-based checkout
- Cash on Delivery
- Multiple-vendor order handling
- Order validation
- Vendor-specific order portions
- Stock verification before order approval
- Automatic inventory deduction after vendor approval
- Customer order confirmation emails

### Email & Notifications

- Transactional emails using Resend
- Vendor order notifications
- Vendor approval emails
- Customer order confirmation emails
- In-app vendor notifications

### Product Images

- Cloudinary support for new product images
- Existing product image support
- Image processing and upload handling

## 🛠️ Technologies Used

- Node.js
- Express.js
- Prisma ORM
- MySQL
- JWT
- Resend
- Cloudinary
- Multer
- Sharp
- Cookie Parser
- CORS

## 📁 Project Structure

```text
zentro-backend/
│
├── config/
├── controllers/
├── middleware/
├── prisma/
├── railway-import/
├── routes/
├── services/
├── uploads/
│   └── products/
│
├── app.js
├── server.js
├── prisma.config.ts
├── package.json
├── package-lock.json
├── zentro-data.sql
├── zentro-data-only.sql
└── .gitignore
```

## 🔐 Environment Variables

The application uses environment variables for sensitive configuration.

Create a `.env` file and configure the required values for:

- Database connection
- JWT secret
- Frontend URL
- Email service
- Cloudinary
- Other deployment-specific configuration


## ▶️ Local Development

Clone the repository:

```bash
git clone https://github.com/mahmad120133548-blip/zentro-backend.git
```

Navigate to the project:

```bash
cd zentro-backend
```

Install dependencies:

```bash
npm install
```

Configure the required environment variables in `.env`.

Generate the Prisma client:

```bash
npx prisma generate
```

Start the development server:

```bash
npm run dev
```

## 🌐 Deployment

The Zentro backend is deployed using **Railway**, with **MySQL** as the production database.

The backend is designed to work with the Zentro frontend deployed separately.

## 🔗 Related Project

**Zentro Frontend:**  
https://github.com/mahmad120133548-blip/zentro-frontend

## 👨‍💻 Author

**Muhammad Ahmad**

Bachelor's in Business and Information Technology  
University of the Punjab

