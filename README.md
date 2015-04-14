# Instructions

Clone this repository and return your implementation as zip (or tar) with .git (we would like to see your commit history :)

Repository contains skeleton of simple Java 8 / Spring Boot based app, which is missing implementation for login functionality. Your task is to implement RESTful API for user login with name and password. There is no single "correct" answer but the API has to fulfill the contract:

* GET /api/login?username={username}&password={password} -> 200 OK with JSON web token in response body, on correct credentials
* GET /api/login/?username={username}&password={password} -> 401 Forbidden, on invalid credentials

Used credentials are: teppo@testaaja.fi/foobar

Architecture of the app should be flexible enough so that fetching users/checking the credentials from external database or API would be easy and doesn't require changes to existing code. For this assignment, external database is not necessary.

# Prerequisites

To run the app you need:

* Java 8
* Maven 3 (https://maven.apache.org/)

# Used libraries in the skeleton

* Spring Boot (http://docs.spring.io/spring-boot/docs/1.2.3.RELEASE/reference/htmlsingle/)
* Java JWT (https://github.com/jwtk/jjwt)
* Mockito (http://mockito.org/)

Feel free to use other libs if you need/like to :)

# Run the tests

`mvn test`

# Start the container/app

`mvn spring-boot:run`

# Clean build

`mvn clean`
