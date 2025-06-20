# REST-API



## 🧰 Programming Language & Framework
- **Language:** Java 17
- **Framework:** Spring Boot 3.5.3

## 🚀 How to Run the Application

1. **Clone the repository**
   ```bash
   git clone https://github.com/umwaribenie/REST-API.git

   ```

2. **Build and run the application**
   ```bash
   ./mvnw spring-boot:run
   ```
   > _Note: Make sure you have Maven Wrapper or Maven installed, and Java 17+ available._

3. **The server will start on**
   ```
   http://localhost:8080
   ```

---

## 🧪 How to Test the API Endpoints

### ➕ Create a User

- **Endpoint:** `POST /users`
- **Request Body:**
  ```json
  {
    "name": "John Doe",
    "email": "john@example.com"
  }
  ```
- **Example `curl` Command:**
  ```bash
  curl -X POST http://localhost:8080/users \
  -H "Content-Type: application/json" \
  -d '{"name":"John Doe","email":"john@example.com"}'
  ```

- **Sample Response:**
  ```json
  {
    "id": "e7e51570-ade3-4cb5-97fd-90576b6a5733",
    "name": "John Doe",
    "email": "john@example.com"
  }
  ```

---

### 🔍 Get a User by ID

- **Endpoint:** `GET /users/{id}`
- **Example `curl` Command:**
  ```bash
  curl http://localhost:8080/users/e7e51570-ade3-4cb5-97fd-90576b6a5733
  ```

- **Sample Response:**
  ```json
  {
    "id": "e7e51570-ade3-4cb5-97fd-90576b6a5733",
    "name": "John Doe",
    "email": "john@example.com"
  }
  ```

- **If User Not Found:**
  ```text
  User not found.
  ```

---

Let me know if you'd like to embed Swagger/OpenAPI instructions too or polish it up with badges and licensing info for public use on GitHub. Always happy to help you shine.
