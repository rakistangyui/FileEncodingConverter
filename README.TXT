========================
BUILD OUTPUT DESCRIPTION
========================

When you build an Java application project that has a main class, the IDE
automatically copies all of the JAR
files on the projects classpath to your projects dist/lib folder. The IDE
also adds each of the JAR files to the Class-Path element in the application
JAR files manifest file (MANIFEST.MF).

To run the project from the command line, go to the dist folder and
type the following:

java -jar "EncodeFile.jar" 

To distribute this project, zip up the dist folder (including the lib folder)
and distribute the ZIP file.

Notes:

* If two JAR files on the project classpath have the same name, only the first
JAR file is copied to the lib folder.
* Only JAR files are copied to the lib folder.
If the classpath contains other types of files or folders, these files (folders)
are not copied.
* If a library on the projects classpath also has a Class-Path element
specified in the manifest,the content of the Class-Path element has to be on
the projects runtime path.
* To set a main class in a standard Java project, right-click the project node
in the Projects window and choose Properties. Then click Run and enter the
class name in the Main Class field. Alternatively, you can manually type the
class name in the manifest Main-Class element.

Arguments
args[0] - Determine if this is a folder by using Y or N flag.
args[1] - Input file or folder
args[2] - Output file or just put NA if you are using the batch conversion
args[3] - Default encoding when the encoding checker fails to check the current encoding of the file.
args[4] - Your desired encoding for the output file.

When you want to convert files inside a folder
java -jar "C:\Users\u108381\Documents\NetBeansProjects\EncodeFile\dist\EncodeFile.jar" Y "D:\Danny" NA ISO-8859-1 x-UTF-16LE-BOM

When you want to convert a single file
java -jar "C:\Users\u108381\Documents\NetBeansProjects\EncodeFile\dist\EncodeFile.jar" N "D:\Danny\Sample.txt" "D:\Danny\Sample_converted.txt" ISO-8859-1 x-UTF-16LE-BOM