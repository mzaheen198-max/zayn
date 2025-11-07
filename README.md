# Hardware Center - Paint E-Commerce App

A modern,e-commerce application for selling paints and painting supplies. Built with React frontend and Node.js/Express backend.

## Features

- 🎨 **Paint-Focused Products**: Browse through various paint categories including Interior, Exterior, Primer, Metal, Wood, Textured, and Waterproofing paints
- 🛒 **Shopping Cart**: Add products to cart, manage quantities, and checkout
- 🔍 **Search Functionality**: Search for products by name, brand, or category
- ⭐ **Product Ratings**: View product ratings and reviews
- 📱 **Responsive Design**: Modern, Amazon-inspired UI that works on all devices
- 💾 **Local Storage**: Cart persists in browser local storage

## Tech Stack

### Frontend
- React 19
- React Router DOM
- CSS3 (Modern styling)

### Backend
- Node.js
- Express.js
- CORS enabled

## Installation & Setup

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn

### Backend Setup

1. Navigate to the backend directory:
```bash
cd backend
```

2. Install dependencies:
```bash
npm install
```

3. Start the backend server:
```bash
npm start
```

The backend will run on `http://localhost:5000`

### Frontend Setup

1. Open a new terminal and navigate to the frontend directory:
```bash
cd frontend
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm start
```

The frontend will run on `http://localhost:3000`

## Project Structure

```
hardware-center/
├── backend/
│   ├── server.js          # Express server with API endpoints
│   └── package.json       # Backend dependencies
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/    # React components
│   │   │   ├── Header.js
│   │   │   ├── HomeBanner.js
│   │   │   ├── ProductCard.js
│   │   │   ├── ProductList.js
│   │   │   └── CategorySection.js
│   │   ├── pages/         # Page components
│   │   │   └── Cart.js
│   │   ├── context/        # React Context
│   │   │   └── CartContext.js
│   │   ├── data/          # Product data
│   │   │   └── products.js
│   │   ├── styles/        # CSS files
│   │   ├── App.js         # Main app component
│   │   └── index.js       # Entry point
│   └── package.json       # Frontend dependencies
└── README.md
```

## API Endpoints

### Products
- `GET /api/products` - Get all products
- `GET /api/products/:id` - Get product by ID
- `GET /api/products?category=Interior Paints` - Filter by category
- `GET /api/products?search=asian` - Search products

### Categories
- `GET /api/categories` - Get all categories

### Cart Tracking (NEW! 🎉)
- `POST /api/cart/add` - Track add to cart event
- `POST /api/cart/remove` - Track remove from cart event
- `POST /api/cart/update` - Track quantity update event
- `POST /api/cart/clear` - Track clear cart event
- `GET /api/cart/analytics` - Get cart analytics and statistics
- `GET /api/cart/events` - Get all cart events (with filters)

### Orders
- `POST /api/orders` - Place an order (also tracks checkout)

### Analytics Dashboard
- Visit `http://localhost:5000/analytics.html` to view real-time cart analytics

## Product Categories

- Interior Paints
- Exterior Paints
- Primer Paints
- Metal Paints
- Wood Paints
- Textured Paints
- Waterproofing

## Usage

1. **Browse Products**: View products organized by category on the homepage
2. **Search**: Use the search bar to find specific products
3. **Add to Cart**: Click "Add to Cart" on any product
4. **View Cart**: Click the cart icon in the header to view your cart
5. **Manage Cart**: Update quantities or remove items from the cart page
6. **Checkout**: Click "Proceed to Checkout" to complete your order

## Features in Detail

### Shopping Cart
- Add multiple products to cart
- Update quantities
- Remove items
- View cart total
- Cart persists in local storage

### Product Display
- Product images
- Brand information
- Ratings and reviews
- Stock status
- Size information
- Price display

### Search
- Real-time search filtering
- Search by product name, brand, or category
- Search results display

## Future Enhancements

- User authentication
- Product detail pages
- Order history
- Payment integration
- Product reviews submission
- Admin dashboard
- Database integration
- Image upload functionality

## License

This project is open source and available for personal use.

## Support

For issues or questions, please check the code or reach out for support.


