HelloMavenProject
This is a basic Java program that prints "Hello, Jenkins + Maven!"
It uses Maven to build the project and Jenkins to automate the build process.

Project Files
Hello_World.java — The Java program file

pom.xml — The Maven build file

The Java code is inside the folder:
src/main/java/Hello_World.java

How to Build and Run
Using Maven locally:
Open a terminal in the project folder.

Run this command:

mvn clean package
You will get a compiled jar file in the target folder.

Using Jenkins:
Start Jenkins 

Open Jenkins in your browser: http://localhost:8080

Go to Manage Jenkins → Tool Configuration and add Maven.

Create a new Freestyle project.

In the build section, choose Invoke top-level Maven targets and put clean package as the Goal.

Save and click Build Now.

Check the console output for BUILD SUCCESS.

What You’ll See
When you run the program, it prints:


[INFO] --- jar:3.4.1:jar (default-jar) @ HelloMavenProject ---
[INFO] Building jar: C:\ProgramData\Jenkins\.jenkins\workspace\Maven_jenkins_intergration\target\HelloMavenProject-1.0-SNAPSHOT.jar
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS

Important
Make sure your Java file is inside src/main/java/ — this is where Maven looks for code.

The project uses Java 8 compatibility.

