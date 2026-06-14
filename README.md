# DecodeLabs Project 3 — Database Integration

## Setup

1. **Install dependencies**
   ```bash
   npm install
   ```

2. **Configure MongoDB Atlas**
   - Open `.env` file
   - Replace the `MONGO_URI` with your actual MongoDB Atlas connection string:
     ```
     MONGO_URI=mongodb+srv://yourUsername:yourPassword@cluster0.xxxxx.mongodb.net/decodelabs_db?retryWrites=true&w=majority
     ```

3. **Run the server**
   ```bash
   npm start
   # OR for development with auto-reload:
   npm run dev
   ```

4. Server runs at: `http://localhost:5000`

---

## API Endpoints

### Users
| Method | Endpoint          | Description      |
|--------|-------------------|------------------|
| GET    | /api/users        | Get all users    |
| GET    | /api/users/:id    | Get user by ID   |
| POST   | /api/users        | Create user      |
| PUT    | /api/users/:id    | Update user      |
| DELETE | /api/users/:id    | Delete user      |

### Products
| Method | Endpoint              | Description          |
|--------|-----------------------|----------------------|
| GET    | /api/products         | Get all products     |
| GET    | /api/products/:id     | Get product by ID    |
| POST   | /api/products         | Create product       |
| PUT    | /api/products/:id     | Update product       |
| DELETE | /api/products/:id     | Delete product       |

---

## Sample Request Bodies

### Create User (POST /api/users)
```json
{
  "name": "Ali Khan",
  "email": "ali@example.com",
  "age": 25,
  "role": "user"
}
```

### Create Product (POST /api/products)
```json
{
  "name": "Laptop",
  "description": "Gaming laptop",
  "price": 150000,
  "category": "Electronics",
  "stock": 10,
  "inStock": true
}
```
