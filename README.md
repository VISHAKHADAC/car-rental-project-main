# 🚗 Car Rental Project

A **web application** that acts as a car rental company.  
Users can:
- View available cars
- Pay for access to selected packages
- Pick up their reserved car

This project was primarily built to learn **JUnit** and **Mockito** testing.

---

## 🛠️ Used Tools & Technologies

- Java 17
- Spring Boot v2.5.5
- Maven v3.8.2
- MySQL Community Server v8.0.27
- Spring Data JPA
- Spring Web MVC
- Spring Security with JWT
- Lombok
- JUnit 5
- Mockito

---

## 📋 Requirements

- **JDK** 1.17
- **Maven** 3.x
- **MySQL Server**

---

## ⚙️ How To Run

### 1️⃣ Install MySQL

Download and install MySQL Community Server if not already installed.

---

### 2️⃣ Clone the repository

```bash
git clone https://github.com/Tomasz3976/car-rental-project.git
```

Navigate to the project directory:

```bash
cd car-rental-project
```

---

### 3️⃣ Configure datasource in `src/main/resources/application.yml`

```yaml
spring:
  datasource:
    url: jdbc:mysql://localhost:3306/carrentaldb
    username: your_mysql_username
    password: your_mysql_password
  jpa:
    hibernate:
      ddl-auto: update
    show-sql: true
```

---

### 4️⃣ Configure datasource in `src/test/resources/application.yml`

```yaml
spring:
  datasource:
    url: jdbc:mysql://localhost:3306/carrentaltestdb
    username: your_mysql_username
    password: your_mysql_password
  jpa:
    hibernate:
      ddl-auto: create-drop
    show-sql: true
```

---

### 5️⃣ Build the project

```bash
mvn clean install
```

---

### 6️⃣ Run the application

```bash
mvn spring-boot:run
```

---

### 7️⃣ Access the application

Server runs at:  
[http://localhost:8080](http://localhost:8080)

---

## 🔐 Login Credentials

| Role   | Username | Password |
|--------|----------|----------|
| User   | user     | user     |
| Manager| manager  | manager  |
| Admin  | admin    | admin    |

---

## 📖 Explore REST APIs

API documentation available via Swagger UI:  
[http://localhost:8080/swagger-ui.html](http://localhost:8080/swagger-ui.html)

---

## 🧪 Testing

This project uses **JUnit 5** and **Mockito** for unit and integration tests.  
To run tests:

```bash
mvn test
```
