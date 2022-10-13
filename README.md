### Description

Simple RESTful application created with **Java** & **Spring**  using Apache Tomcat. This application can be treated as a microservice with a simple database as a List\<E\> which stores a list of *people* entries that can be editted.

### Features
- Add, delete, modify people entries.
- Retrieve list of people.

### Instructions

`GET localhost:8080/api/v1/person`
- Retrieves all people.

`GET localhost:8080/api/v1/person/{id}`
- Retrieves single person entry with specified id.

`POST localhost:8080/api/v1/person`
```json
{
    "name": "John Doe"
}
```
- Creates a person entry and adds them to the database generating a unique UUID with the name specified in the JSON body above.

`PUT localhost:8080/api/v1/person/{id}`
```json
{
    "name": "John Doe"
}
```
- Modifies the persons name with {id} to the name "John Doe" if they exist.


`DELETE localhost:8080/api/v1/person/{id}`

- Deletes person with specified id.
