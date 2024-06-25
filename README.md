# SimpleTicketManager

STM is a robust task management system built using Spring Boot and PrimeFaces. It allows users to manage their tasks efficiently with features such as authentication, CRUD operations for tasks, task assignment, and categorization.

## Features

- **User Authentication**: Secure login and registration.
- **Task Management**: Create, read, update, and delete tasks.
- **User Assignment**: Assign tasks to specific users.
- **Task Categorization**: Organize tasks into categories.
- **PrimeFaces Integration**: Interactive UI components.

## Getting Started

### Prerequisites

- Java 17
- Maven
- H2 Database (for development)
- PostgreSQL (for production)
- Heroku CLI (for deployment on Heroku)

### Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/yourusername/TaskFlow.git
    cd TaskFlow
    ```

2. **Build the project:**

    ```bash
    mvn clean install
    ```

3. **Run the application:**

    ```bash
    mvn spring-boot:run
    ```

4. **Access the application:**

   Open your browser and go to `http://localhost:8080`

### Configuration

#### Database Configuration

- **Development**: Uses H2 database by default.
- **Production**: Configure PostgreSQL or any other preferred database.

Update the `application.properties` file for production database settings:

```properties
# PostgreSQL settings
spring.datasource.url=jdbc:postgresql://<your-database-url>:5432/<your-database-name>
spring.datasource.username=<your-database-username>
spring.datasource.password=<your-database-password>
spring.jpa.hibernate.ddl-auto=update
