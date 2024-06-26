![image](https://github.com/Strange1108/SmartContactManager/assets/137171724/8b07bfad-8ef3-4795-ac6f-644b8865ffc4)
![image](https://github.com/Strange1108/SmartContactManager/assets/137171724/fce3239d-698a-4184-ade0-6a11e5b3c2a5)
![image](https://github.com/Strange1108/SmartContactManager/assets/137171724/38692bfd-4e00-45fe-a515-6ea94a7250cd)
![image](https://github.com/Strange1108/SmartContactManager/assets/137171724/11996be0-07c6-42b4-b024-74814eac46ee) 
![image](https://github.com/Strange1108/SmartContactManager/assets/137171724/88d18fa9-8b39-4ebc-b66f-edb8c5f1726d)






# Contact Management System

This learning project aims to create an efficient contact management application that provides a smarter way of handling contacts with full authentication and authorization features. The project utilizes Spring Boot with Thymeleaf and follows the MVC architecture. For authentication and authorization, Spring Security is employed.

## Technologies Used

- **Backend:**
  - [Spring Boot](https://spring.io/projects/spring-boot) - Develops the back-end.
  - [Spring Data JPA](https://spring.io/projects/spring-data-jpa) - Performs Database CRUD operations.

- **Frontend:**
  - [HTML5](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/HTML5) - Markup language.
  - [CSS3](https://developer.mozilla.org/en-US/docs/Archive/CSS3) - Stylesheet language.
  - [Bootstrap](https://getbootstrap.com/) - Front-end framework.
  - [Thymeleaf](https://www.thymeleaf.org/) - Template engine.

- **Database:**
  - [SQLite3](https://www.sqlite.org/index.html) - Embedded database generating a .db file.

## Data Flow
  ### Model
  The `model` package contains the two main classes:
  - Contact
  - User
      
  ### Controller
  - The `controller` package includes the following controllers:
  - HomeController 
  - UserController
  - SearchController
  - ForgetController

  ### Services
  - The services are as follows:
  - EmailService

  ### Repository
  - The `repo` package contains repository interfaces that extend `JpaRepository` for each model. The interface names are structured as follows:
  - UserRepository
  - ContactRepository
    
## Project Overview

### Learning Project with Spring Boot and Thymeleaf
- **Objective:** Create an application for efficient contact management.
- **Authentication:** Implemented using Spring Security.
- **Backend:** Developed using Spring Boot, with Spring Data JPA for database operations.
- **Frontend:** HTML5, CSS3, Bootstrap, and Thymeleaf used for the user interface.

### Contact Management System
- **Objective:** Manage details of Remainder, Mobiles, Phone Numbers, People, and Addresses.
- **Technology Stack:** HTML, CSS, JavaScript, Java, Spring Boot, MySQL.
- **Database:** MySQL is used for storing contact-related information.
- **Access Control:** Only administrators have guaranteed access to the system.

In management terminology, this advanced contact management system serves as an Individual Resource Management (IRM) tool. It helps manage an individual's interactions with current and future contacts, organizing, collaborating, and synchronizing health, lifestyle, and financial needs.

## Running the Application

1. Clone the repository.
   ```bash
   git clone https://github.com/Strange1108/SmartContactManager.git
   cd SmartContactManager
