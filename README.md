# Java MYSQL CRUD

The project was built in Java 17 using maven and Spring-Boot.

Packages used include Lombok and JSON Simple.

## Getting started
Install a local instance of MySQL in your machine.
Create a new db called user_database.

Change the first three lines of **/src/resources/application.properties** with the appropriate data for your local db  installation.

Install dependencies by running 

```terminal
mnv install
```
Run the project with 
```terminal
mvn spring-boot:run
```
## CRUD OPERATIONS

**GET** all users at

```terminal
http://localhost:8080/api/users
```
**GET ONE** user with

```terminal
http://localhost:8080/api/users/{id}
```

**POST** user at

```terminal
http://localhost:8080/api/users
```
sending
```json
{
    "firstName": "John",
    "lastName": "Doe",
    "email": "johndoe@example.com"
}
```
**PUT** existing user at

```terminal
http://localhost:8080/api/users/{id}
```
sending
```json
{
    "firstName": "John",
    "lastName": "Doe",
    "email": "johndoe@example.com"
}
```
**DELETE** an user at
```terminal
http://localhost:8080/api/users/{id}
```