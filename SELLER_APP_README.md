# Hardware Center - Seller Dashboard

A complete seller/admin dashboard for managing products, orders, and analytics for the Hardware Center paint store.

## Features

### 🔐 Authentication
- Secure login system
- Session management
- Protected routes

### 📊 Dashboard
- Real-time statistics
- Total products, orders, revenue
- Today's orders and revenue
- Pending and completed orders

### 📦 Product Management
- View all products
- Add new products
- Edit existing products
- Delete products
- Product categories management

### 🛒 Order Management
- View all orders
- Update order status (Pending, Processing, Completed, Cancelled)
- Real-time order updates
- Order details and items

### 📈 Analytics
- Order status breakdown
- Sales by category
- Top selling products
- Revenue insights

## Setup Instructions

### 1. Install Dependencies

```bash
cd frontend-seller
npm install
```

### 2. Start the Seller Dashboard

```bash
npm start
```

The seller dashboard will run on `http://localhost:3001` (or next available port)

### 3. Login Credentials

**Email:** `seller@hardwarecenter.com`  
**Password:** `seller123`

## Backend API Endpoints

All seller endpoints are prefixed with `/api/seller`

### Authentication
- `POST /api/seller/login` - Seller login

### Dashboard
- `GET /api/seller/dashboard/stats` - Get dashboard statistics

### Products
- `GET /api/seller/products` - Get all products
- `POST /api/seller/products` - Add new product
- `PUT /api/seller/products/:id` - Update product
- `DELETE /api/seller/products/:id` - Delete product

### Orders
- `GET /api/seller/orders` - Get all orders
- `GET /api/seller/orders/:id` - Get single order
- `PUT /api/seller/orders/:id/status` - Update order status

### Analytics
- `GET /api/seller/analytics` - Get analytics data

## Project Structure

```
frontend-seller/
├── src/
│   ├── components/
│   │   ├── Header.js
│   │   ├── Header.css
│   │   ├── Sidebar.js
│   │   └── Sidebar.css
│   ├── pages/
│   │   ├── Login.js
│   │   ├── Login.css
│   │   ├── Dashboard.js
│   │   ├── Dashboard.css
│   │   ├── Products.js
│   │   ├── Products.css
│   │   ├── Orders.js
│   │   ├── Orders.css
│   │   ├── Analytics.js
│   │   └── Analytics.css
│   ├── App.js
│   ├── App.css
│   └── index.js
└── package.json
```

## Usage

### Adding a Product

1. Navigate to **Products** page
2. Click **+ Add Product** button
3. Fill in product details:
   - Name, Category, Price, Size
   - Brand, Image URL
   - Description, Features
   - Stock status
4. Click **Add Product**

### Managing Orders

1. Navigate to **Orders** page
2. View all orders with details
3. Change order status using the dropdown
4. Orders auto-refresh every 5 seconds

### Viewing Analytics

1. Navigate to **Analytics** page
2. View:
   - Order status breakdown
   - Sales by category
   - Top selling products

## Important Notes

⚠️ **Security**: In production:
- Use proper password hashing (bcrypt)
- Implement JWT tokens for authentication
- Add role-based access control
- Use a database instead of in-memory storage
- Add input validation and sanitization

## Integration with Main App

The seller dashboard connects to the same backend as the customer app:
- Backend runs on `http://localhost:5000`
- Orders placed by customers appear in seller dashboard
- Products added by sellers appear in customer app

## Next Steps

- Add product image upload
- Add bulk product import/export
- Add email notifications for new orders
- Add advanced filtering and search
- Add reports export (PDF/Excel)
- Add inventory management
- Add customer management

## Support

For issues or questions, check the backend server is running and accessible at `http://localhost:5000`.

