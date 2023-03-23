# Core-Java


## 1) JVM

JVM is an abstract machine. Read-only .class file. 
The JVM has two primary functions: the "write once, run anywhere" principle, and to manage and optimizing program memory. 
JVM is platform-dependent.  
{Class loader: It is the subsystem of JVM that is used to load class files.}
JVM Fallow three notations specification, implementation, and instance.
   JVM:
Load’s code -> Verifies code -> Executes code -> Provides runtime environment.
always find the main method  -> if not found then throws an exception  ->	no main method found

a) java is Interpreted? -> yes.


## 2) JRE	
JVM, JRE, and JDK are platform-dependent. 
Java is platform-independent.
JRE refers to a runtime environment in which JAVA bytecode can be executed.
it's an implementation of the JVM which physically exists.

<picture>
  <source media="(prefers-color-scheme: light)" srcset="https://user-images.githubusercontent.com/73180409/226957816-1b4fa937-0cf0-4c1a-a395-cd83f7d431c9.png">
  
</picture>

![jdk-jvm]()

## 3) JDK
JDK stands for Java Development Kit or sometimes it is also referred to as Java Standard Edition Development Kit. 
It is the tool necessary to compile and package Java programs.
JDK is a development environment to develop a wide range of applications such as desktop applications, web applications 

## 4) Features of Java or Java buzzwords

simple
Object-oriented	
portable	
independent	secured	
robust	
Architectural natural	
dynamic
High Performance	
Multithreaded	
Distributed

What happens at runtime? 
Class file -> class Loader->byte code verified -> Interpreter -> Runtime -> hardware.

Class loader: It is the subsystem of JVM that is used to load class files.
Bytecode Verifier: Checks the code fragments for illegal code.
Interpreter: Read bytecode Stream then execute the instructions.


## 6) Public static void main(String[] args)

### public:  
the keyword is an access modifier that represents visibility. It means it is visible to all class.

### static: 
is a keyword. The main () method is executed by the JVM, so it doesn't require creating an object to invoke the main () method. So, it saves memory.
We must declare the main() function static as no class object is present when the java runtime starts.

### void: 
is the return type of the method. It means it doesn't return any value.

### MAIN: 
is the name of a method. And the starting point of the program.

String [] args ---> command line args. meaning is  Array of String type.

## 7) System.out.println():

	System: class
	out:the object of Print Stream class--printing purpose.
	println: method of Print Stream class.

## 8) Java provides three types of control flow statements.
### Decision-Making statements: 
a)if statements b) switch statement

### Loop statements:
a) Do-while loop b) while loop c) for loop d) for-each loop.

### Jump statements
a) break statement b) continue statement



