# NZ Store Backend

The backend API server for the NZ Store project, providing product filtering and cart management functionality.

## 🚀 Features

- 🔍 Filter products via API
- 🛒 Cart management system
- 🔄 Real-time synchronization with frontend
- 🌍 CORS-enabled for cross-origin requests

## 🧱 Technology

- Node.js
- Express.js
- RESTful API architecture

## 🚀 Deployment Guide (Glitch)

1. Create a Glitch account at https://glitch.com
2. Create a new project
3. Import this GitHub repo or upload the files manually
4. Your API will be live at your Glitch project URL

## 🖥️ Local Development

1. Clone the repository
2. Install dependencies:
   ```
   npm install
   ```
3. Start the server:
   ```
   npm start
   ```
4. The API will be available at http://localhost:3000

## 🔌 API Documentation

### Product Filtering

```bash
# Filter products by category and brand
POST /api/filter
Content-Type: application/json

{
  "category": "Phones",
  "brand": "Samsung"
}

# Get current filter
GET /api/filter
```

### Cart Management

```bash
# Add products to cart by name
POST /api/cart/named
Content-Type: application/json

{
  "names": ["Samsung A23", "LG WashPro"]
}

# Get current cart
GET /api/cart

# Reset cart
POST /api/cart/reset
```

## 📝 Data Structure

The API uses the following product structure:

```javascript
{
  name: "Product Name",
  category: "Category",
  brand: "Brand",
  details: "Product details",
  price: "$Price"
}
```

## Frontend Repository

The frontend for this project is available at [nz-store-frontend](https://github.com/rxd-blue/nz-store-frontend) 