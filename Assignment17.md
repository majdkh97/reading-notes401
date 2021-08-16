# Read17

## Spring Boot and OAuth2


### OAuth2

**OAuth2 is an authorization framework that enables the application Web Security to access the resources from the client. To build an OAuth2 application, we need to focus on the Grant Type (Authorization code), Client ID and Client secret.**

**Gradle users can add the following dependencies in the build.gradle file.**
- compile('org.springframework.boot:spring-boot-starter-security')
- compile('org.springframework.boot:spring-boot-starter-web')
- testCompile('org.springframework.boot:spring-boot-starter-test')
- testCompile('org.springframework.security:spring-security-test')
- compile("org.springframework.security.oauth:spring-security-oauth2")
- compile('org.springframework.security:spring-security-jwt')
- compile("org.springframework.boot:spring-boot-starter-jdbc")
- compile("com.h2database:h2:1.4.191")  

**where**
- Spring Boot Starter Security − Implements the Spring Security

- Spring Security OAuth2 − Implements the OAUTH2 structure to enable the Authorization Server and Resource Server.

- Spring Security JWT − Generates the JWT Token for Web security

- Spring Boot Starter JDBC − Accesses the database to ensure the user is available or not.

- Spring Boot Starter Web − Writes HTTP endpoints.

- H2 Database − Stores the user information for authentication and authorization.


### Securing the Application with GitHub and Spring Security
**To make the application secure**
- you can simply add Spring Security as a dependency.
- since you’re wanting to do a "social" login (delegate to GitHub),
- you should include the Spring Security OAuth 2.0 Client starter:

### You need to configure your app to use GitHub as the authentication provider. To achieve this, do the following:
- Add a New GitHub app
- Configure application.yml
- Boot up the application

