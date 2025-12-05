# Product API with Swagger

A simple REST API for managing products with Swagger documentation.

## Installation

```bash
npm install
```

## Running the API

```bash
npm start
```

For development with auto-reload:
```bash
npm run dev
```

## API Documentation

Once the server is running, visit:
- API Docs: http://localhost:3000/api-docs

## Endpoints

- `GET /api/products` - Get all products
- `GET /api/products/:id` - Get product by ID
- `POST /api/products` - Create a new product
- `PUT /api/products/:id` - Update a product
- `DELETE /api/products/:id` - Delete a product

## Example Request

```bash
curl -X POST http://localhost:3000/api/products \
  -H "Content-Type: application/json" \
  -d '{"name":"Tablet","price":499.99,"category":"Electronics"}'
```
