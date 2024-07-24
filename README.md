# GCF_w1
Zero to one

Step 1: Clone the repo
Step 2: To build JoularJX, you need Java 11+ and Maven, then just build: [refering to the joularjx-develop folder]

```
mvn clean install -DskipTests
```

Alternatively, you can use the Maven wrapper shipped with the project with the command:

```
Linux: ./mvnw clean install -DskipTests
Windows: ./mvnw.cmd clean install -DskipTests
```
Step 3: JoularJX is a Java agent where you can simply hook it to the Java Virtual Machine when starting your Java program's main class:

```
java -javaagent:joularjx-$version.jar YourProgramMainClass
```

If your program is a JAR file, then just run it as usual while adding JoularJX:

```
java -javaagent:joularjx-$version.jar -jar yourProgram.jar
```

JoularJX will generate multiple CSV files according to the configuration settings (in ```config.properties```), and will create these files in a ```joularjx-results```folder.
# Change to your own local path
In this case, run java -javaagent:C:\Users\*\.m2\repository\org\noureddine\joularjx\3.0.0\joularjx-3.0.0.jar -jar C:\Users\*\spring-petclinic-3.2.0-SNAPSHOT.jar

Step 4: The App is booted on localhost:8080. Add a pet to any owner and CTRL+C to stop the Joularjx the joularjx-results folder will be updated.

Step 5: Execute the GUI in C:\Users\*\GCF_w1\ReleaseJoularGUI\Release\net6.0-windows10.0.19041.0\joularjx-gui by double clicking. Below will be shown:
![image](https://github.com/user-attachments/assets/b53590e2-db2d-4383-a12d-62b83b92ae7a)


Step 6: Select the folder and click Analysis button.
![image](https://github.com/user-attachments/assets/c2faffcf-8e4b-47af-8827-ce11a3011661)

Step 7: Select any of the PID to view the visual display:
![image](https://github.com/user-attachments/assets/047cfec9-e248-4759-a6a8-9d2543e804e6)
![image](https://github.com/user-attachments/assets/068d4dbc-4579-4923-be63-2b4fe0bbbd66)


