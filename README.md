# Job Application REST API

A Spring Boot REST API for managing job postings.  
This project supports full CRUD (Create, Read, Update, Delete) operations using RESTful endpoints.

---

## Tech Stack
- Java
- Spring Boot
- Spring Data JPA
- Hibernate
- H2 In-Memory Database
- Postman (API testing)

---

## Features
- Create a job posting
- Retrieve all job postings
- Retrieve a job posting by ID
- Update an existing job posting
- Delete a job posting
- Uses an in-memory H2 database for easy local testing

---

## API Endpoints

| Method  | Endpoint       | Description |
|--------|---------------|-------------|
| GET    | /jobs          | Retrieve all job postings |
| GET    | /jobs/{id}     | Retrieve a job posting by ID |
| POST   | /jobs          | Create a new job posting |
| PUT    | /jobs/{id}     | Update an existing job posting |
| DELETE | /jobs/{id}     | Delete a job posting |

---

## Sample Request (POST /jobs)

```json
{
  "title": "Software Engineer",
  "description": "Backend role using Java and Spring Boot",
  "minSalary": "80000",
  "maxSalary": "120000",
  "location": "New York"
}
Project Structure
bash
Copy code
src/
 └── main/
      └── java/
           └── com/rifah/firstjobapp/
                ├── job/
                │    ├── Job.java
                │    ├── JobController.java
                │    ├── JobRepository.java
                │    └── JobService.java
                └── job/impl/
                     └── JobServiceImpl.java
Controller: Handles HTTP requests and responses

Service: Contains business logic

Repository: Manages database operations using JPA

Entity: Represents the Job data model

