# Student Data API (REST API learning project)

Simple Spring Boot RESTful APIs that manages student data.

## Stack

- Java 25
- Spring Boot 4.0.3
- Spring Web MVC + Spring Data JPA
- MySQL
- Maven Wrapper

### Prerequisites

- JDK 25
- MySQL running
- Database: `studentsdb`

### Start app

Windows:

```bash
mvnw.cmd spring-boot:run
```

macOS/Linux:

```bash
./mvnw spring-boot:run
```

Base URL: `http://localhost:8080/api`

## API

Base path: `/api/students`

- `GET /api/students` - list all students
- `GET /api/students/{id}` - get student by id
- `POST /api/students` - create student
- `PUT /api/students/{id}` - update student
- `PATCH /api/students/{id}` - partial update (`name`, `email`)
- `DELETE /api/students/{id}` - delete student

Sample create request:

```json
{
  "name": "Alice Johnson",
  "email": "alice@example.com"
}
```

## Config

Copy values from `application.properties.example` into `src/main/resources/application.properties` and set your DB credentials.

