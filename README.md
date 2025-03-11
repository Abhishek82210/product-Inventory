🛍️ Product Inventory API

📌 A Spring Boot REST API for managing a product inventory.
Supports CRUD operations (Create, Read, Update, Delete) on products stored in a MySQL database.
🚀 Features

✅ Add new products
✅ Retrieve all products or a single product
✅ Update product details
✅ Delete products
✅ Uses MySQL for persistent storage
✅ Follows RESTful API principles
🛠️ Tech Stack

    Backend: Spring Boot (Spring MVC, Spring Data JPA)
    Database: MySQL
    Build Tool: Maven
    Language: Java

📂 Project Structure

product-inventory-api/
│── src/main/java/com/example/productinventory/
│   ├── controller/   # API Controllers
│   ├── model/        # Entity Classes
│   ├── repository/   # JPA Repositories
│   ├── service/      # Business Logic
│── src/main/resources/
│   ├── application.properties  # Configuration File
│── pom.xml  # Maven Dependencies
│── README.md  # Project Documentation

⚙️ Setup & Installation
1️⃣ Prerequisites

Make sure you have installed:
✅ Java 17+ ( or more )
✅ Maven
✅ MySQL Server
2️⃣ Clone the Repository

git clone https://github.com/your-username/product-inventory-api.git
cd product-inventory-api

3️⃣ Configure MySQL Database

Update src/main/resources/application.properties with your database details:

spring.datasource.url=jdbc:mysql://localhost:3306/productdb
spring.datasource.username=your-username
spring.datasource.password=your-password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true

4️⃣ Build & Run the Project

mvn clean install
mvn spring-boot:run

📌 API Endpoints
Method	Endpoint	Description
GET	/products	Get all products
GET	/products/{id}	Get product by ID
POST	/products	Add a new product
PUT	/products/{id}	Update product by ID
DELETE	/products/{id}	Delete product by ID
📝 Sample JSON Request (Create Product)

{
  "name": "Laptop",
  "price": 75000,
  "quantity": 10
}
