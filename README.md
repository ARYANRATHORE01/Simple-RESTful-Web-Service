# 🌐 Simple RESTful Web Service (Spring Boot CRUD API)

A lightweight **Spring Boot REST API** project built to demonstrate basic **CRUD (Create, Read, Update, Delete)** operations.  
This application manages a list of items (like books, products, etc.) using **Spring Boot**, **Spring Data JPA**, and simple REST endpoints.

---

## 🚀 Features

- ✅ Create, Read, Update, and Delete items  
- 📦 RESTful endpoints returning JSON  
- ⚙️ Simple service and repository layers  
- 🧩 Uses Spring Boot starter modules (Web + JPA)  
- 🧠 Beginner-friendly, modular, and extendable  

---

## 🧠 Skills Covered

| Area | Technology |
|------|-------------|
| Framework | Spring Boot |
| API Design | RESTful APIs |
| CRUD Operations | GET, POST, PUT, DELETE |
| ORM | Spring Data JPA |
| Build Tool | Maven |
| IDE | IntelliJ IDEA / VS Code |
| Language | Java 17+ |

---

## 📁 Project Structure

rest-crud-main/
├── rest-crud/
│ ├── src/
│ │ ├── main/
│ │ │ ├── java/com/example/restcrud/
│ │ │ │ ├── Item.java
│ │ │ │ ├── ItemController.java
│ │ │ │ ├── ItemRepository.java
│ │ │ │ └── RestCrudApplication.java
│ │ │ └── resources/
│ │ │ ├── application.properties
│ │ │ └── items.http
│ ├── pom.xml
│ └── .gitignore
└── README.md

yaml
Copy code

---

## ⚙️ How to Run Locally

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/aryanrathore01/Simple-RESTful-Web-Service.git
cd Simple-RESTful-Web-Service/rest-crud
2️⃣ Build the Project
bash
Copy code
./mvnw clean install
3️⃣ Run the Application
bash
Copy code
./mvnw spring-boot:run
By default, the app runs at:
👉 http://localhost:8080

🔗 REST API Endpoints
Method	Endpoint	Description
GET	/api/items	Get all items
GET	/api/items/{id}	Get item by ID
POST	/api/items	Create a new item
PUT	/api/items/{id}	Update existing item
DELETE	/api/items/{id}	Delete item by ID

🧾 Example JSON Request (POST)
json
Copy code
{
  "name": "Java Programming Book",
  "price": 499.0,
  "quantity": 10
}
🧠 Example Response
json
Copy code
{
  "id": 1,
  "name": "Java Programming Book",
  "price": 499.0,
  "quantity": 10
}
🧩 application.properties Example
properties
Copy code
server.port=8080
spring.datasource.url=jdbc:h2:mem:testdb
spring.datasource.driverClassName=org.h2.Driver
spring.datasource.username=sa
spring.datasource.password=
spring.jpa.hibernate.ddl-auto=update
spring.h2.console.enabled=true
Access H2 Console:
👉 http://localhost:8080/h2-console

🧭 Future Enhancements
Add Swagger for interactive API documentation

Integrate with MySQL or PostgreSQL

Add input validation and error handling

Create a frontend using React or Angular

👨‍💻 Author
Aryan Rathore
🌐 ARYANRATHORE01

📜 License
This project is created for learning and demonstration purposes.
You are free to use, modify, or enhance it for educational or personal projects.
