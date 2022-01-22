# Spring Boot REST API

## With basic **CRUD** funtionality
- Create user
- Read user(s)
- Update user
- Delete user

## Written in Java
App hosted, with some changes, on [Heroku](https://www.heroku.com/):
- [Here](https://guarded-sands-40052.herokuapp.com/) (don't forget the `/api/users` endpoint)

## Database
RDS hosted with [Amazon Relational Database Service (RDS)](https://aws.amazon.com/rds/)

## Installation

Clone the repository to your local machine and from the project root build using [Maven](https://maven.apache.org/what-is-maven.html)

Run `mvn clean install -X` to get a `.jar` file, which you can run from the `./target` directory like this:
```
java -jar springboot-crud-rest-aws-0.0.1-SNAPSHOT.jar
```

If you're having issues with [CORS](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS), you may need to enable CORS by editing your `UserController.java` file like so:

```
@RestController
@CrossOrigin(origins = "https://your-front-end.app")
@RequestMapping("/api/users")
public class UserController {
```
Importing `import org.springframework.web.bind.annotation.CrossOrigin;`

## Ending GIF

Ask <a href="mailto:joe@holyculture.org">Joe Johnson</a> if you have any questions!

![Workout Gif](https://media1.giphy.com/media/MAiBgTnLfH3Nrj68eA/giphy.gif?cid=790b7611aa02621d8511aa93f0e56bb02561970c20e6b43c&rid=giphy.gif&ct=g)
