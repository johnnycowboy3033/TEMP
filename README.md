# TEMP

[Full Stack ReactJS with Spring Boot](https://www.youtube.com/watch?v=-LUA-LHXobE)


**Terminate the Application in Eclipse:**

 Open Eclipse and go to the Console view.

 Look for the Spring Boot application that's running.

 Click the Terminate button (red square) on the top right corner of the Console view.

**Identify and Kill the Process Manually:**

 If the application didn't stop, you can identify the process using the port.

 On Windows: Open Command Prompt and run:

SH
```
netstat -ano | findstr <Port Number>
```

Replace <Port Number> with the port number your Spring Boot application is using (e.g., 8080).

This will show you the process ID (PID) using that port.

Then, run:

SH
```
taskkill /F /PID <PID>
```
Replace <PID> with the actual process ID.

**Change the Port in Your Spring Boot Application:**

To avoid port conflicts in the future, you can change the port your Spring Boot application uses.

Open the application.properties or application.yml file in your project.

Add or modify the following line:

properties
```
server.port=8081
```

Save the file and restart your application.
