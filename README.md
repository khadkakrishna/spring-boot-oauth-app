# spring-boot-oauth-app

### Prerequisites:
1. generate google-oauth client-id and client-secret
2. generate github-oauth client-id and client-secret
> Note: After generating the above tokens place it in `src/main/resources/application.properties`
 
### About the application:
* The starting point of the application is `src/main/java/com/development/SpringOAuthApplication/SpringOAuthApplication.java` that runs the spring boot application.
* There is one rest-controller defined in `src/main/java/com/development/SpringOAuthApplication/controller/Controller.java` that lands to the `http://localhost:8080/` and prints Hello.
* The configuration for authentications are defined in  `src/main/java/com/development/SpringOAuthApplication/config/WebSecurityConfig.java` for the OAuth2 login as well as Form Based login. 
* The `UserDetailsService` is defined in `src/main/java/com/development/SpringOAuthApplication/config/WebSecurityConfig.java` that adds the user for the login with username:user and password:password.

### Running the application:
To run the application, type `mvn spring-boot:run` on terminal

The application will be accessible at `http://localhost:8080` and redirected to the login page at `http://localhost:8080/login`

> Note: To run the application in debug mode add `debug=true` in `src/main/resources/application.properties`