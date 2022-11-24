# <img src="taksi.jpg" width="5%"> TAXI SERVICE

Web application that allows authenticated users to keep records of cars and drivers for small Taxi services. 

Allows you to display a list of cars, manufacturers and drivers. It is possible to add new  
manufacturers with the indication of the country production, add new vehicles with model and manufacturer.   
Maintain a list, add, remove drivers, as well as attach / detach drivers to a specific car.

### Technologies
* Maven
* Dependency injection
* Java Servlet
* JSP
* Tomcat
* N-tier architecture
* JDBC (MySQL)

### Project structure  
Project structure is represented by N-tier architecture and consists of the following levels:
* web
* model
* service
* dao

_The Web layer_ is based on JSP and Servlet technologies (controllers).  
Apache Tomcat 9 was chosen as the web server, it is also responsible for the life cycle of servlets.

_The model level_ is represented in the following diagram:

<img src="taxi_models_diagram.jpeg" width = 50%>

_The service layer_ contains a set of interfaces and their implementations, such as:
* handling to the DAO level
* authentication
* validation

And _the DAO layer_ works with a relational database (MySQL 8) via JDBC

### Demo

To demonstrate the project, you need to install the MySQL database server ([instruction](https://dev.mysql.com/doc/mysql-installation-excerpt/5.7/en/)). <br>
Create database with [sql script](src/main/resources/init_db.sql) <br>
[Download and install](https://tomcat.apache.org/download-90.cgi) Apache Tomcat 9<br>
Configure and start the web server
