# SpringBootMusic

- Install Eclipse Web Developer from here <a href="https://www.eclipse.org/downloads/">Click here</a>

- Click on File > Import  
![image](https://user-images.githubusercontent.com/54632221/179565571-dcdcce7b-ab32-4b8d-ad2f-06f170e5cbae.png)

- Select Git > Smart Import <br/>
![image](https://user-images.githubusercontent.com/54632221/179565942-12af98e7-0549-423b-ba6a-c39a329461cc.png)

- Enter your Github URI of the repository > Select the Branch > Select the Directory to clone the repository > Click on Finish

![image](https://user-images.githubusercontent.com/54632221/179566577-60176a7b-0b7c-46f1-bc4a-d99c0ad6275a.png)

- Go to src/main/resources/application.properties add your Database Configuration of MySQL

- Go to src/main/java/com/example/music/MusicApplication/MusicApplication.java and run it has Java Application

- Your Backend Server will run on localhost:8082

- To disable Cors for your application make sure you change the URL of the restConfiguration in each of the controller files
![image](https://user-images.githubusercontent.com/54632221/179567658-10670a8f-3892-4849-8a90-1c067e8e9170.png)

- If Spring Security asks for User Credentials for the backend server add these lines to src/main/resources/application.properties file
```
spring.security.user.name=user
spring.security.user.password=1234
```

- Run this MYSQL queries in your local DB instance
```
Create database MusicApp;
use MusicApp;
Create table ARTIST (id int primary key auto_increment,name varchar(255), dob varchar(255), Bio varchar(1024));
Create table SONGS (id int primary key auto_increment, name varchar(255), dateofrelease varchar(255), picByte varbinary(1000));
Create table USER(id int primary key auto_increment, name varchar(255), email varchar(255));

```
