📚 Book API – Spring Boot CRUD Project
This project was developed as part of the DWF404 – Web Application Development with Frameworks course at Universidad Don Bosco.
The objective is to build a basic REST API for the fictional publisher "Letras Vivas" to manage its book catalog.

👨‍💻 Team Members
David Alvarez – AM240104 (Repository Owner: @DavidAlvar3z)

Ashley Valdez – VG240979 (Collaborator: @achi-vonz)

🚀 Features
The API provides the following functionalities:

List all books

Add a new book

Search books by title

Delete a book

Additionally, the project includes:

Layered architecture (Controller, Service, Repository, Model)

Spring Data JPA for persistence

Dependency Injection using @Autowired

Configuration through application.properties

Basic API documentation with Swagger

🛠️ Technologies Used
Java 17

Spring Boot 3.x

Spring Data JPA

H2 Database (in-memory)

Swagger (Springdoc OpenAPI)

Maven

📥 How to Clone the Repository
To get a copy of this project locally, follow these steps:

bash
Copiar
Editar
# Clone the repository
git clone https://github.com/DavidAlvar3z/DWF-Desafio01.git

# Navigate into the project folder
cd DWF-Desafio01
▶️ How to Run the Project
Make sure you have Java 17 and Maven installed.

Open the project in your IDE (IntelliJ IDEA or Eclipse recommended).

Run the following command in the terminal:

bash
Copiar
Editar
mvn spring-boot:run
The application will start on http://localhost:8080 by default.

📄 Swagger Documentation
Swagger UI is available after running the project.
Access it at:

bash
Copiar
Editar
http://localhost:8080/swagger-ui.html
This allows you to test all endpoints directly from the browser.

🔧 Endpoints Overview
Method	Endpoint	Description
GET	/api/books	List all books
POST	/api/books	Add a new book
GET	/api/books/{title}	Search books by title
DELETE	/api/books/{id}	Delete a book by ID

⚙️ Configuration
Edit src/main/resources/application.properties to change port or database configurations:

properties
Copiar
Editar
server.port=8080
spring.datasource.url=jdbc:h2:mem:booksdb
spring.datasource.driverClassName=org.h2.Driver
spring.datasource.username=sa
spring.datasource.password=
spring.jpa.hibernate.ddl-auto=update
🏆 Extra Improvements
Input validation for required fields

Centralized error handling using @ControllerAdvice

Swagger UI integration for better documentation

📌 Academic Information
Course: DWF404 – Web Application Development with Frameworks

Teacher: Miguel Alejandro Meléndez Martínez

University: Universidad Don Bosco (UDB)

Year: 2025 – Cycle 2

Group: 01L
