# 📌 Instagram Backend Application  
**Java | Spring Boot | Maven | MySQL | REST API**  

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)  

---

## 📖 Overview  
The **Instagram Backend Application# 📌 Instagram Backend Application  
**Java | Spring Boot | Maven | MySQL | REST API**  

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)  

---

## 📖 Overview  
The **Instagram Backend Application** is a **scalable Spring Boot-based backend** designed for a social media platform with features similar to Instagram.  
It provides a **comprehensive set of RESTful API endpoints** for:
- **User management** (Registration, Authentication, Profile Management)  
- **Post creation & retrieval**  
- **Commenting & liking**  
- **Security & authentication** using **Spring Security**  

This application follows a **robust architecture** ensuring clean code, modular design, and seamless database integration.  

---

## 🛠 Technologies Used  
- **Framework:** Spring Boot  
- **Language:** Java 21  
- **Database:** MySQL  
- **Build Tool:** Apache Maven  
- **Documentation:** SpringDoc OpenAPI (Swagger UI)  
- **Security:** Spring Security  
- **Email Handling:** JavaMail API  

---

## 📌 Dependencies  

### 1️⃣ **Spring Boot Starter Data JPA**  
**Purpose:** Simplifies database operations using Spring Data repositories.  
```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-data-jpa</artifactId>
</dependency>


2️⃣ Spring Boot Starter Web
Purpose: Provides support for building RESTful web applications.

<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-web</artifactId>
</dependency>

3️⃣ Spring Security
Purpose: Implements authentication & authorization.

<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-security</artifactId>
</dependency>

4️⃣ MySQL Connector/J
Purpose: JDBC driver for MySQL database connection.

<dependency>
    <groupId>mysql</groupId>
    <artifactId>mysql-connector-java</artifactId>
    <scope>runtime</scope>
</dependency>

5️⃣ Spring Boot Starter Validation
Purpose: Ensures request data validation.

<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-validation</artifactId>
</dependency>

6️⃣ Swagger (Springdoc OpenAPI)
Purpose: API documentation and testing.

<dependency>
    <groupId>org.springdoc</groupId>
    <artifactId>springdoc-openapi-starter-webmvc-ui</artifactId>
    <version>2.0.2</version>
</dependency>

7️⃣ JavaMail API
Purpose: Email notifications & account verification.

<dependency>
    <groupId>javax.mail</groupId>
    <artifactId>mail</artifactId>
    <version>1.4.7</version>
</dependency>

📌 Project Structure

📂 Instagram-Backend
 ├── 📁 src/main/java/com/instagram
 │   ├── 📁 controller      # REST API Controllers
 │   ├── 📁 service         # Business logic & services
 │   ├── 📁 repository      # JPA Repository Interfaces
 │   ├── 📁 model           # Entities (User, Post, Comment, Like)
 │   ├── 📁 security        # Spring Security Configurations
 │   ├── 📁 exception       # Custom Exceptions & Handlers
 │   ├── 📄 InstagramBackendApplication.java  # Main Application Class
 ├── 📁 src/main/resources
 │   ├── 📄 application.properties  # Database & App Configuration
 ├── 📄 pom.xml  # Project Dependencies
 ├── 📄 README.md  # Documentation


📌 Data Flow
1️⃣ User Registration & Authentication

Users register using email & password
Credentials are securely stored (hashed passwords)
Users authenticate via JWT tokens managed by Spring Security

2️⃣ User Profile Management

Users can update username, profile picture, bio

3️⃣ Post Creation & Retrieval

Users can create, update, delete, and view posts
Posts include images, captions, timestamps


4️⃣ Commenting on Posts

Users can add, update, and delete comments on posts


5️⃣ Liking Posts

Users can like/unlike posts and view total likes


6️⃣ Security & Authentication

Spring Security ensures secure API access
Passwords are hashed & authentication tokens are validated


7️⃣ Data Persistence

Data stored in MySQL database using Spring Data JPA

📌 RESTful API Endpoints

🔹 User Management
Method	                  Endpoint	                         Description
POST	             /api/users/register	                 Register a new user
POST	             /api/users/login	                     Authenticate user & return JWT token
GET	               /api/users/{userId}	                 Retrieve user profile
PUT	              /api/users/{userId}	                   Update user profile
DELETE	          /api/users/{userId}	                   Delete user account

🔹 Post Management
Method              Endpoint	                    Description
POST	           /api/posts	                    Create a new post
GET	            /api/posts	                    Retrieve all posts
GET	            /api/posts/{postId}	            Retrieve a specific post
PUT	            /api/posts/{postId}	            Update a post
DELETE	       /api/posts/{postId}	            Delete a post

🔹 Comment Management

Method	                  Endpoint	                 Description
POST	             /api/comments	                  Add a comment
GET	              /api/comments/{postId}	        Get comments for a post
PUT	             /api/comments/{commentId}	     Update a comment
DELETE	        /api/comments/{commentId}	       Delete a comment

🔹 Like Management

Method	               Endpoint	            Description
POST	              /api/likes/{postId}	   Like a post
GET	                /api/likes/{postId}	  Get likes for a post
DELETE	            /api/likes/{postId}	  Unlike a post

📌 Database Schema

Table Name	               Description
users           	Stores user accounts & profiles
posts           	Stores posts with images & captions
comments        	Stores user comments on posts
likes           	Tracks likes on posts
followers       	Manages user follow relationships

📌 Database Configuration (MySQL)
Modify application.properties to set up MySQL:

spring.datasource.url=jdbc:mysql://localhost:3306/InstagramDB
spring.datasource.username=your_username# 📌 Instagram Backend Application  
**Java | Spring Boot | Maven | MySQL | REST API**  

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)  

---

## 📖 Overview  
The **Instagram Backend Application** is a **scalable Spring Boot-based backend** designed for a social media platform with features similar to Instagram.  
It provides a **comprehensive set of RESTful API endpoints** for:
- **User management** (Registration, Authentication, Profile Management)  
- **Post creation & retrieval**  
- **Commenting & liking**  
- **Security & authentication** using **Spring Security**  

This application follows a **robust architecture** ensuring clean code, modular design, and seamless database integration.  

---

## 🛠 Technologies Used  
- **Framework:** Spring Boot  
- **Language:** Java 21  
- **Database:** MySQL  
- **Build Tool:** Apache Maven  
- **Documentation:** SpringDoc OpenAPI (Swagger UI)  
- **Security:** Spring Security  
- **Email Handling:** JavaMail API  

---

## 📌 Dependencies  

### 1️⃣ **Spring Boot Starter Data JPA**  
**Purpose:** Simplifies database operations using Spring Data repositories.  
```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-data-jpa</artifactId>
</dependency>


2️⃣ Spring Boot Starter Web
Purpose: Provides support for building RESTful web applications.

<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-web</artifactId>
</dependency>

3️⃣ Spring Security
Purpose: Implements authentication & authorization.

<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-security</artifactId>
</dependency>

4️⃣ MySQL Connector/J
Purpose: JDBC driver for MySQL database connection.

<dependency>
    <groupId>mysql</groupId>
    <artifactId>mysql-connector-java</artifactId>
    <scope>runtime</scope>
</dependency>

5️⃣ Spring Boot Starter Validation
Purpose: Ensures request data validation.

<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-validation</artifactId>
</dependency>

6️⃣ Swagger (Springdoc OpenAPI)
Purpose: API documentation and testing.

<dependency>
    <groupId>org.springdoc</groupId>
    <artifactId>springdoc-openapi-starter-webmvc-ui</artifactId>
    <version>2.0.2</version>
</dependency>

7️⃣ JavaMail API
Purpose: Email notifications & account verification.

<dependency>
    <groupId>javax.mail</groupId>
    <artifactId>mail</artifactId>
    <version>1.4.7</version>
</dependency>

📌 Project Structure

📂 Instagram-Backend
 ├── 📁 src/main/java/com/instagram
 │   ├── 📁 controller      # REST API Controllers
 │   ├── 📁 service         # Business logic & services
 │   ├── 📁 repository      # JPA Repository Interfaces
 │   ├── 📁 model           # Entities (User, Post, Comment, Like)
 │   ├── 📁 security        # Spring Security Configurations
 │   ├── 📁 exception       # Custom Exceptions & Handlers
 │   ├── 📄 InstagramBackendApplication.java  # Main Application Class
 ├── 📁 src/main/resources
 │   ├── 📄 application.properties  # Database & App Configuration
 ├── 📄 pom.xml  # Project Dependencies
 ├── 📄 README.md  # Documentation


📌 Data Flow
1️⃣ User Registration & Authentication

Users register using email & password
Credentials are securely stored (hashed passwords)
Users authenticate via JWT tokens managed by Spring Security

2️⃣ User Profile Management

Users can update username, profile picture, bio

3️⃣ Post Creation & Retrieval

Users can create, update, delete, and view posts
Posts include images, captions, timestamps


4️⃣ Commenting on Posts

Users can add, update, and delete comments on posts


5️⃣ Liking Posts

Users can like/unlike posts and view total likes


6️⃣ Security & Authentication

Spring Security ensures secure API access
Passwords are hashed & authentication tokens are validated


7️⃣ Data Persistence

Data stored in MySQL database using Spring Data JPA

📌 RESTful API Endpoints

🔹 User Management
Method	                  Endpoint	                         Description
POST	             /api/users/register	                 Register a new user
POST	             /api/users/login	                     Authenticate user & return JWT token
GET	               /api/users/{userId}	                 Retrieve user profile
PUT	              /api/users/{userId}	                   Update user profile
DELETE	          /api/users/{userId}	                   Delete user account

🔹 Post Management
Method              Endpoint	                    Description
POST	           /api/posts	                    Create a new post
GET	            /api/posts	                    Retrieve all posts
GET	            /api/posts/{postId}	            Retrieve a specific post
PUT	            /api/posts/{postId}	            Update a post
DELETE	       /api/posts/{postId}	            Delete a post

🔹 Comment Management

Method	                  Endpoint	                 Description
POST	             /api/comments	                  Add a comment
GET	              /api/comments/{postId}	        Get comments for a post
PUT	             /api/comments/{commentId}	     Update a comment
DELETE	        /api/comments/{commentId}	       Delete a comment

🔹 Like Management

Method	               Endpoint	            Description
POST	              /api/likes/{postId}	   Like a post
GET	                /api/likes/{postId}	  Get likes for a post
DELETE	            /api/likes/{postId}	  Unlike a post

📌 Database Schema

Table Name	               Description
users           	Stores user accounts & profiles
posts           	Stores posts with images & captions
comments        	Stores user comments on posts
likes           	Tracks likes on posts
followers       	Manages user follow relationships

📌 Database Configuration (MySQL)
Modify application.properties to set up MySQL:

spring.datasource.url=jdbc:mysql://localhost:3306/InstagramDB
spring.datasource.username=your_username
spring.datasource.password=your_password
spring.datasource.driverClassName=com.mysql.cj.jdbc.Driver
spring.jpa.database-platform=org.hibernate.dialect.MySQLDialect
Make sure MySQL is running and credentials are correctly set.

📌 License
This project is licensed under the GNU General Public License v3.0.

📬 Contact
📧 Email: atulupa@12345@gmail.com
🐙 GitHub: https://github.com/Upadhyay123a/

spring.datasource.password=your_password
spring.datasource.driverClassName=com.mysql.cj.jdbc.Driver
spring.jpa.database-platform=org.hibernate.dialect.MySQLDialect
Make sure MySQL is running and credentials are correctly set.

📌 License
This project is licensed under the GNU General Public License v3.0.

📬 Contact
📧 Email: atulupa@12345@gmail.com
🐙 GitHub: https://github.com/Upadhyay123a/
** is a **scalable Spring Boot-based backend** designed for a social media platform with features similar to Instagram.  
It provides a **comprehensive set of RESTful API endpoints** for:
- **User management** (Registration, Authentication, Profile Management)  
- **Post creation & retrieval**  
- **Commenting & liking**  
- **Security & authentication** using **Spring Security**  

This application follows a **robust architecture** ensuring clean code, modular design, and seamless database integration.  

---

## 🛠 Technologies Used  
- **Framework:** Spring Boot  
- **Language:** Java 21  
- **Database:** MySQL  
- **Build Tool:** Apache Maven  
- **Documentation:** SpringDoc OpenAPI (Swagger UI)  
- **Security:** Spring Security  
- **Email Handling:** JavaMail API  

---

## 📌 Dependencies  

### 1️⃣ **Spring Boot Starter Data JPA**  
**Purpose:** Simplifies database operations using Spring Data repositories.  
```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-data-jpa</artifactId>
</dependency>


2️⃣ Spring Boot Starter Web
Purpose: Provides support for building RESTful web applications.

<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-web</artifactId>
</dependency>

3️⃣ Spring Security
Purpose: Implements authentication & authorization.

<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-security</artifactId>
</dependency>

4️⃣ MySQL Connector/J
Purpose: JDBC driver for MySQL database connection.

<dependency>
    <groupId>mysql</groupId>
    <artifactId>mysql-connector-java</artifactId>
    <scope>runtime</scope>
</dependency>

5️⃣ Spring Boot Starter Validation
Purpose: Ensures request data validation.

<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-validation</artifactId>
</dependency>

6️⃣ Swagger (Springdoc OpenAPI)
Purpose: API documentation and testing.

<dependency>
    <groupId>org.springdoc</groupId>
    <artifactId>springdoc-openapi-starter-webmvc-ui</artifactId>
    <version>2.0.2</version>
</dependency>

7️⃣ JavaMail API
Purpose: Email notifications & account verification.

<dependency>
    <groupId>javax.mail</groupId>
    <artifactId>mail</artifactId>
    <version>1.4.7</version>
</dependency>

📌 Project Structure

📂 Instagram-Backend
 ├── 📁 src/main/java/com/instagram
 │   ├── 📁 controller      # REST API Controllers
 │   ├── 📁 service         # Business logic & services
 │   ├── 📁 repository      # JPA Repository Interfaces
 │   ├── 📁 model           # Entities (User, Post, Comment, Like)
 │   ├── 📁 security        # Spring Security Configurations
 │   ├── 📁 exception       # Custom Exceptions & Handlers
 │   ├── 📄 InstagramBackendApplication.java  # Main Application Class
 ├── 📁 src/main/resources
 │   ├── 📄 application.properties  # Database & App Configuration
 ├── 📄 pom.xml  # Project Dependencies
 ├── 📄 README.md  # Documentation


📌 Data Flow
1️⃣ User Registration & Authentication

Users register using email & password
Credentials are securely stored (hashed passwords)
Users authenticate via JWT tokens managed by Spring Security

2️⃣ User Profile Management

Users can update username, profile picture, bio

3️⃣ Post Creation & Retrieval

Users can create, update, delete, and view posts
Posts include images, captions, timestamps


4️⃣ Commenting on Posts

Users can add, update, and delete comments on posts


5️⃣ Liking Posts

Users can like/unlike posts and view total likes


6️⃣ Security & Authentication

Spring Security ensures secure API access
Passwords are hashed & authentication tokens are validated


7️⃣ Data Persistence

Data stored in MySQL database using Spring Data JPA

📌 RESTful API Endpoints

🔹 User Management
Method	                  Endpoint	                         Description
POST	             /api/users/register	                 Register a new user
POST	             /api/users/login	                     Authenticate user & return JWT token
GET	               /api/users/{userId}	                 Retrieve user profile
PUT	              /api/users/{userId}	                   Update user profile
DELETE	          /api/users/{userId}	                   Delete user account

🔹 Post Management
Method              Endpoint	                    Description
POST	           /api/posts	                    Create a new post
GET	            /api/posts	                    Retrieve all posts
GET	            /api/posts/{postId}	            Retrieve a specific post
PUT	            /api/posts/{postId}	            Update a post
DELETE	       /api/posts/{postId}	            Delete a post

🔹 Comment Management

Method	                  Endpoint	                 Description
POST	             /api/comments	                  Add a comment
GET	              /api/comments/{postId}	        Get comments for a post
PUT	             /api/comments/{commentId}	     Update a comment
DELETE	        /api/comments/{commentId}	       Delete a comment

🔹 Like Management

Method	               Endpoint	            Description
POST	              /api/likes/{postId}	   Like a post
GET	                /api/likes/{postId}	  Get likes for a post
DELETE	            /api/likes/{postId}	  Unlike a post

📌 Database Schema

Table Name	               Description
users           	Stores user accounts & profiles
posts           	Stores posts with images & captions
comments        	Stores user comments on posts
likes           	Tracks likes on posts
followers       	Manages user follow relationships

📌 Database Configuration (MySQL)
Modify application.properties to set up MySQL:

spring.datasource.url=jdbc:mysql://localhost:3306/InstagramDB
spring.datasource.username=your_username# 📌 Instagram Backend Application  
**Java | Spring Boot | Maven | MySQL | REST API**  

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)  

---

## 📖 Overview  
The **Instagram Backend Application** is a **scalable Spring Boot-based backend** designed for a social media platform with features similar to Instagram.  
It provides a **comprehensive set of RESTful API endpoints** for:
- **User management** (Registration, Authentication, Profile Management)  
- **Post creation & retrieval**  
- **Commenting & liking**  
- **Security & authentication** using **Spring Security**  

This application follows a **robust architecture** ensuring clean code, modular design, and seamless database integration.  

---

## 🛠 Technologies Used  
- **Framework:** Spring Boot  
- **Language:** Java 21  
- **Database:** MySQL  
- **Build Tool:** Apache Maven  
- **Documentation:** SpringDoc OpenAPI (Swagger UI)  
- **Security:** Spring Security  
- **Email Handling:** JavaMail API  

---

## 📌 Dependencies  

### 1️⃣ **Spring Boot Starter Data JPA**  
**Purpose:** Simplifies database operations using Spring Data repositories.  
```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-data-jpa</artifactId>
</dependency>


2️⃣ Spring Boot Starter Web
Purpose: Provides support for building RESTful web applications.

<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-web</artifactId>
</dependency>

3️⃣ Spring Security
Purpose: Implements authentication & authorization.

<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-security</artifactId>
</dependency>

4️⃣ MySQL Connector/J
Purpose: JDBC driver for MySQL database connection.

<dependency>
    <groupId>mysql</groupId>
    <artifactId>mysql-connector-java</artifactId>
    <scope>runtime</scope>
</dependency>

5️⃣ Spring Boot Starter Validation
Purpose: Ensures request data validation.

<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-validation</artifactId>
</dependency>

6️⃣ Swagger (Springdoc OpenAPI)
Purpose: API documentation and testing.

<dependency>
    <groupId>org.springdoc</groupId>
    <artifactId>springdoc-openapi-starter-webmvc-ui</artifactId>
    <version>2.0.2</version>
</dependency>

7️⃣ JavaMail API
Purpose: Email notifications & account verification.

<dependency>
    <groupId>javax.mail</groupId>
    <artifactId>mail</artifactId>
    <version>1.4.7</version>
</dependency>

📌 Project Structure

📂 Instagram-Backend
 ├── 📁 src/main/java/com/instagram
 │   ├── 📁 controller      # REST API Controllers
 │   ├── 📁 service         # Business logic & services
 │   ├── 📁 repository      # JPA Repository Interfaces
 │   ├── 📁 model           # Entities (User, Post, Comment, Like)
 │   ├── 📁 security        # Spring Security Configurations
 │   ├── 📁 exception       # Custom Exceptions & Handlers
 │   ├── 📄 InstagramBackendApplication.java  # Main Application Class
 ├── 📁 src/main/resources
 │   ├── 📄 application.properties  # Database & App Configuration
 ├── 📄 pom.xml  # Project Dependencies
 ├── 📄 README.md  # Documentation


📌 Data Flow
1️⃣ User Registration & Authentication

Users register using email & password
Credentials are securely stored (hashed passwords)
Users authenticate via JWT tokens managed by Spring Security

2️⃣ User Profile Management

Users can update username, profile picture, bio

3️⃣ Post Creation & Retrieval

Users can create, update, delete, and view posts
Posts include images, captions, timestamps


4️⃣ Commenting on Posts

Users can add, update, and delete comments on posts


5️⃣ Liking Posts

Users can like/unlike posts and view total likes


6️⃣ Security & Authentication

Spring Security ensures secure API access
Passwords are hashed & authentication tokens are validated


7️⃣ Data Persistence

Data stored in MySQL database using Spring Data JPA

📌 RESTful API Endpoints

🔹 User Management
Method	                  Endpoint	                         Description
POST	             /api/users/register	                 Register a new user
POST	             /api/users/login	                     Authenticate user & return JWT token
GET	               /api/users/{userId}	                 Retrieve user profile
PUT	              /api/users/{userId}	                   Update user profile
DELETE	          /api/users/{userId}	                   Delete user account

🔹 Post Management
Method              Endpoint	                    Description
POST	           /api/posts	                    Create a new post
GET	            /api/posts	                    Retrieve all posts
GET	            /api/posts/{postId}	            Retrieve a specific post
PUT	            /api/posts/{postId}	            Update a post
DELETE	       /api/posts/{postId}	            Delete a post

🔹 Comment Management

Method	                  Endpoint	                 Description
POST	             /api/comments	                  Add a comment
GET	              /api/comments/{postId}	        Get comments for a post
PUT	             /api/comments/{commentId}	     Update a comment
DELETE	        /api/comments/{commentId}	       Delete a comment

🔹 Like Management

Method	               Endpoint	            Description
POST	              /api/likes/{postId}	   Like a post
GET	                /api/likes/{postId}	  Get likes for a post
DELETE	            /api/likes/{postId}	  Unlike a post

📌 Database Schema

Table Name	               Description
users           	Stores user accounts & profiles
posts           	Stores posts with images & captions
comments        	Stores user comments on posts
likes           	Tracks likes on posts
followers       	Manages user follow relationships

📌 Database Configuration (MySQL)
Modify application.properties to set up MySQL:

spring.datasource.url=jdbc:mysql://localhost:3306/InstagramDB
spring.datasource.username=your_username
spring.datasource.password=your_password
spring.datasource.driverClassName=com.mysql.cj.jdbc.Driver
spring.jpa.database-platform=org.hibernate.dialect.MySQLDialect
Make sure MySQL is running and credentials are correctly set.

📌 License
This project is licensed under the GNU General Public License v3.0.

📬 Contact
📧 Email: atulupa@12345@gmail.com
🐙 GitHub: https://github.com/Upadhyay123a/

spring.datasource.password=your_password
spring.datasource.driverClassName=com.mysql.cj.jdbc.Driver
spring.jpa.database-platform=org.hibernate.dialect.MySQLDialect
Make sure MySQL is running and credentials are correctly set.

📌 License
This project is licensed under the GNU General Public License v3.0.

📬 Contact
📧 Email: atulupa@12345@gmail.com
🐙 GitHub: https://github.com/Upadhyay123a/
