# Topic

A forum to discuss and collaborate views on a various topics where users can create topics, post comments in one to many fashion and search topics. This project exhibits a 3-tier architecture modeling such as Web, App and Database which is simple and robust. Primary objective of this project is to unviel power of REST architecture built using Spring framework and persisted on MongoDB.

## Architecture

## Technology stack

| Feature                 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| Technology &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;    |
|-----------------------  |-------------------------------|
| Language                | Java                          |
| Database                | MongoDB                       |
| Logging                 | Logback                       |
| JWT                     | Access tokens                 |
| Auto configuration      | Spring boot                   |
| Persistence             | Spring Data                   |
| API                     | Spring REST                   |
| AOP                     | Spring AOP                    |
| Security                | Spring Security               |

> ### Why MongoDB?
> 1. High reads without any joins as in relational database.
> 2. Easy for development as it often involves modification of data structure(schema)
> 3. More understandable No-SQL queries.

> ### Why Spring framework?
> Spring has highly organised modules for various software architecture concerns.

> #### Spring boot
> 1. Provides cloud native support.
> 2. Easy kick start of application using Starter dependencies.
> 3. Out of box features like Dev tools, actuators and auto configurations.
> 4. Embedded servers.

> #### Persistence - Spring Data 
> 1. MongoRepository provides high level abstraction on the MongoClient from Mongo driver jar.
> 2. Elimination of boiler plate code.

> #### API - Spring REST
> 1. Annotation driven REST API
> 2. Seamless integration with other spring modules.

> #### AOP  - Spring
> 1. Application's cross cutting concerns like logging and refresh tokens handling, has been flesh out from core business logic.
> 2. Used CGlib proxies for logging, since JDK Proxies can be applied only on interface implementations.

> #### Security -  Spring Security
> 1. Spring Security provides out of the box functionalities for securing endpoints based on filters.
> 2. It also provides Bcrypt password hashing which is been persisted in the database.
> 3. Decryption of the received AES - 256 bits encrypted password.

> ### Logging - Logback
> Simple logging configuration
