========================
BUILD OUTPUT DESCRIPTION
========================

When you build an Java application project that has a main class, the IDE
automatically copies all of the JAR
files on the projects classpath to your projects dist/lib folder. The IDE
also adds each of the JAR files to the Class-Path element in the application
JAR files manifest file (MANIFEST.MF).

Ensure that you have Java installed: JAR files require Java to be installed on your system. 
You can verify if Java is installed by opening a terminal or command prompt and running the following command:

java --version
If Java is installed, you will see the version information.
If not, you will need to download and install Java from the official website (https://www.java.com).

Locate the JAR file: Find the JAR file you want to run on your computer. Make sure you know its file path.

Open a terminal or command prompt: Open a terminal or Navigate to the directory containing the JAR file:
Run the JAR file in command prompt: Once you are in the directory containing the JAR file, use the following command to run it:

java -jar <filename>.jar

Replace <filename> with the actual name of the JAR file. 

java -jar CrossNKnot.jar

Press Enter to execute the command: After entering the command, press Enter, and Java will execute the JAR file.
To run the project directly:
download the jar file and if any other lib folder and un the jar file. It will execute as an exe file.
