# Springboot_Java_mavenproject1_usingmysql
This project demonstrates a simple Spring Boot application integrated with MySQL to perform basic CRUD operations using RESTful APIs.

## Requirements
Java JDK (8 or later)
Maven
MySQL Server

## Setup

### Clone the Repository:

Copy code
```
git clone https://github.com/SankarshanMishra/Springboot_Java_mavenproject1_usingmysql.git
```
### Configure MySQL Database:

Create a MySQL database named demo_db.

Update application.properties in src/main/resources with your MySQL database configuration:

properties
```
spring.datasource.url=jdbc:mysql://localhost:3306/demo_db
spring.datasource.username=your_username
spring.datasource.password=your_password
```
### Build and Run:

#### Navigate to the project directory:


Copy code
```
cd Springboot_Java_mavenproject1_usingmysql
```
#### Build the project using Maven:

Copy code
```
mvn clean install
```
#### Run the application:


Copy code
```
mvn spring-boot:run
```
## Endpoints

### 1. Add a New User
#### URL: POST /demo/add
#### Request Body:
json
Copy code
```
{
  "name": "John Doe",
  "email": "johndoe@example.com"
}
```
#### Response:
json
Copy code
```
{
  "id": 1,
  "name": "John Doe",
  "email": "johndoe@example.com"
}
```
### 2. Get All Users
#### URL: GET /demo/all
#### Response:
json
Copy code
```
[
  {
    "id": 1,
    "name": "John Doe",
    "email": "johndoe@example.com"
  },
  {
    "id": 2,
    "name": "Jane Smith",
    "email": "janesmith@example.com"
  }
]
```
## Technologies Used
Spring Boot
Spring Data JPA
MySQL Database

## Contributing
Contributions are welcome! Fork this repository and submit a pull request with your enhancements.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

