# elwasys Web Portal

![Screenshot](https://raw.githubusercontent.com/kabieror/elwasys-portal/master/docs/screenshot-dashboard.png)

## Set up a Development Environment

The following tool stack is recommended:

-	Java Development Kit 8
	http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html

-	Apache Maven
	https://maven.apache.org/

-	IntelliJ IDEA
	https://www.jetbrains.com/idea/

## Start the development server

### From the command line

```
mvn jetty:run
```

### Within IntelliJ:

1. Run > Edit Configurations...
2. Click the Plus icon
3. Select "Maven"
4. Set the working directory to be the root of the repository
5. Set "Command line" to "jetty:run"
6. Click "OK"
7. Select the Run Configuration you just created and click the start arrow.

The web portal will be listening on port 8080. Access it via http://localhost:8080.
