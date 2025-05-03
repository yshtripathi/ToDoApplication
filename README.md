# ✅ ToDoApplication

A simple and efficient To-Do list application built using Java and Spring Boot. This application allows users to manage their tasks effectively by providing functionalities to create, read, update, and delete to-do items.

---

## 📋 Features

- **Add Tasks**: Create new to-do items with titles and descriptions.
- **View Tasks**: Retrieve a list of all existing to-do items.
- **Update Tasks**: Modify existing to-do items.
- **Delete Tasks**: Remove to-do items that are no longer needed.

---

## 🛠️ Technologies Used

- **Java 17**
- **Spring Boot 3.x**
- **Spring MVC**
- **Spring Data JPA**
- **H2 Database** (for development and testing)
- **Maven** (for project management)

---

## 🚀 Getting Started

### Prerequisites

Ensure you have the following installed:

- Java 17 or higher
- Maven 3.x

### Installation

```bash
git clone https://github.com/yshtripathi/ToDoApplication.git
cd ToDoApplication
```

### Build and Run

```bash
mvn clean install
mvn spring-boot:run
```

Open your browser and go to:

```
http://localhost:8080
```

---

## 📁 Project Structure

```
ToDoApplication/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/
│   │   │       └── example/
│   │   │           └── todo/
│   │   │               ├── controller/
│   │   │               │   └── TodoController.java
│   │   │               ├── model/
│   │   │               │   └── Todo.java
│   │   │               ├── repository/
│   │   │               │   └── TodoRepository.java
│   │   │               └── ToDoApplication.java
│   │   └── resources/
│   │       ├── application.properties
│   │       └── templates/
│   │           └── index.html
├── pom.xml
```

---

## 🔧 Configuration

```properties
spring.datasource.url=jdbc:h2:mem:todoapp
spring.datasource.driverClassName=org.h2.Driver
spring.datasource.username=sa
spring.datasource.password=
spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
spring.h2.console.enabled=true
```

Visit the H2 console at:

```
http://localhost:8080/h2-console
```

Use JDBC URL: `jdbc:h2:mem:todoapp`

---

## 📬 API Endpoints

- `GET /api/todos` - Retrieve all to-dos
- `GET /api/todos/{id}` - Retrieve by ID
- `POST /api/todos` - Create a to-do
- `PUT /api/todos/{id}` - Update a to-do
- `DELETE /api/todos/{id}` - Delete a to-do

---

## 🧪 Testing

```bash
mvn test
```

---

## 🤝 Contributing

Contributions are welcome! Fork the repo and submit a pull request.

---

## 📄 License

MIT License. See the [LICENSE](LICENSE) file.

---

## 👤 Author

Developed by [Yash Tripathi](https://github.com/yshtripathi)
