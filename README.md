# Spring MVC with Thymeleaf Lab

This lab guides you through creating a simple Spring Boot web application using Spring MVC and Thymeleaf.

## Prerequisites

- Java JDK 11 or higher
- Maven or Gradle
- IDE (IntelliJ, Eclipse, VS Code)
- Basic Java, HTML, CSS knowledge

## Objectives

- Setup Spring Boot project with Spring MVC & Thymeleaf
- Understand MVC architecture
- Create controllers & handle requests
- Use model to pass data to views
- Create dynamic views with Thymeleaf
- Process form submissions with validation

## Project Setup

Use [Spring Initializr](https://start.spring.io/):

- Group: `com.example`
- Artifact: `spring-thymeleaf-lab`
- Dependencies: Spring Web, Thymeleaf, Spring Boot DevTools, Validation
- Java Version: 17

## Project Structure

```
src/main/java/com/example/springthymeleaflab/
├── SpringThymeleafLabApplication.java
├── controllers/
│   ├── HomeController.java
│   └── StudentController.java
├── models/
│   └── Student.java
src/main/resources/
├── application.properties
├── templates/
│   ├── home.html
│   └── students/
│       ├── list.html
│       └── register.html
├── static/
```

## Application Flow

### Home Page

- URL: `/`
- Controller: `HomeController`
- View: `home.html` (uses `th:text="${message}"`)

### Student Management

- List Students: `/students/list`
- Register Student: `/students/register`
- Model: `Student` (with validation annotations)

### Templates

- `home.html`: Welcome page
- `students/list.html`: Lists all registered students
- `students/register.html`: Registration form with validation

## Run the App

Run via IDE or `mvn spring-boot:run` and open `http://localhost:8080`.

## Notes

- Uses in-memory `List<Student>` for demo purposes
- No database integration

---

© 2025 sihem – Spring Boot Thymeleaf Lab
