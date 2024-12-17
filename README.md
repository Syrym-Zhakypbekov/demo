# Final Examination Project Description

## **Slide 1: Project Overview**
- **Title:** Simple Spring Boot CRUD Application
- **Objective:**
  - Create a Spring Boot project.
  - Give to the project your NAME and context of the your project
  - Upload the project to GitHub
  - Show your Repository to the Examinator
- **Freedom of Choice:**
  - Use **Maven** or **Gradle** (recommended: Maven).
  - Use **Java 17** (recommended).
  - You may also use **Kotlin** if preferred.

---

## **Slide 2: Key Technologies to Use**
- **Spring Boot:** Framework for building Java applications.
- **H2 Database:** In-memory database for simplicity.
- **Spring Data JPA:** Simplified database operations.
- **Lombok:** Reduces boilerplate code.
- **Git & GitHub:** Project must be uploaded to a GitHub repository.
- **IDE:** Recommended IDEs include IntelliJ IDEA, Eclipse, or VS Code.

---

## **Slide 3: Project Requirements**
1. **Basic CRUD Application**:
   - Develop a simple application to manage a resource
2. **Layers to Implement:**
   - **Model**: Represent your data
   - **Repository**: Use JPA to interact with H2 database.
   - **Service**: Add business logic
   - **Controller**: Handle HTTP requests (GET, POST, etc.).
3. **Dependencies:**
   - Spring Web
   - Spring Data JPA
   - Lombok
   - H2 Database
4. **Configuration:**
   - Use `application.properties` to configure H2 database.
   - Enable H2 Console for testing.

  ```properties
  # H2 Database Configuration

  spring.datasource.url=jdbc:h2:file:./data/testdb
  spring.datasource.driverClassName=org.h2.Driver
  spring.datasource.username=sa
  spring.datasource.password=
  
  # Hibernate DDL configuration
  spring.jpa.hibernate.ddl-auto=update
  spring.jpa.show-sql=true
  
  # H2 Console Configuration
  spring.h2.console.enabled=true
  spring.h2.console.path=/h2-console
  ```

---

## **Slide 4: Sample Database Schema**
- Resource: **RandomTableName**
  - **Fields:**
    - `id` (Primary Key, Long, Auto-generated)
    - `name` (String)
    - `email` (String)
- Example:
   | id | name       | email              |
   |----|------------|--------------------|
   | 1  | Arman Cheburekov   | a.cheburek@baursak.kz   |
   | 2  | Kraven the Hunter | kraven@marvel.com   |

---

## **Slide 5: Application Endpoints**
1. **GET **
   - Retrieves the list of all *****.
2. **POST / **
   - Adds a new ******* to the database.
3. **Example Input (POST):**
   ```json
   {
       "name": "Arman Cheburekov",
       "email": "a.cheburek@baursak.kz"
   }
   ```

---

## **Slide 6: H2 Database Configuration**
- Use the following properties in `application.properties`:
   ```properties
   # H2 Database Configuration
  spring.datasource.url=jdbc:h2:file:./data/testdb
  spring.datasource.driverClassName=org.h2.Driver
  spring.datasource.username=sa
  spring.datasource.password=
  
  # Hibernate DDL configuration
  spring.jpa.hibernate.ddl-auto=update
  spring.jpa.show-sql=true
  
  # H2 Console Configuration
  spring.h2.console.enabled=true
  spring.h2.console.path=/h2-console
   ```
- **H2 Console Access**:
   - URL: `http://localhost:8080/h2-console`
   - JDBC URL: `jdbc:h2:file:./data/testdb`
   - Username: `sa`
   - Password: (leave blank).

---

## **Slide 7: Submission Guidelines**
1. **Project Naming**:
   - Name the project whatever you want.
2. **GitHub Repository**:
   - Push the project to your personal GitHub repository.
   - Ensure the repository is public or share the link.
3. **Checklist Before Exam**:
   - Project compiles and runs without errors.
   - All endpoints are working as expected.
   - Project is available on GitHub.

---

## **Slide 8: Evaluation Criteria**
1. **Project Structure** (25%)
   - Proper implementation of Model, Repository, Service, and Controller.
2. **Code Quality** (20%)
   - Use of Lombok, clean code practices, and proper annotations.
3. **Functionality** (30%)
   - CRUD operations are functional.
4. **Database Integration** (15%)
   - H2 Database setup and integration with Spring Data JPA.
5. **GitHub Submission** (10%)
   - Project successfully uploaded to GitHub.

---

## **Slide 9: Exam Day Instructions**
- Come to the exam with:
   1. **GitHub repository link**.
   2. Your project ready on your computer.
   3. IDE set up to demonstrate the project.
- Be prepared to:
   - Explain your code.
   - Run the project and test endpoints.
   - Show database functionality in H2 Console.
   - Be READY To PASS the test Junit

---


