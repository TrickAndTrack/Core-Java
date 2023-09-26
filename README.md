# Core-Java


## 1) JVM

JVM is an abstract machine. Read-only .class file. means Byte code.
The JVM has two primary functions: the "write once, run anywhere" principle, and to manage and optimizing program memory. 
JVM is platform-dependent. so example is you can not run jvm on IOS so JVM need to be build for a perticular OS.
{Class loader: It is the subsystem of JVM that is used to load class files.}
JVM Fallow three notations specification, implementation, and instance.
JVM: Load’s code -> Verifies code -> Executes code -> Provides runtime environment.
always find the main method  -> if not found then throws an exception  ->	no main method found.

a) java is Interpreted? -> yes.
![image](https://github.com/TrickAndTrack/Core-Java/assets/73180409/2c62f7ee-788d-4d42-95d1-90a2c1c3e770)


## 2) JRE	

JRE refers to a runtime environment in which JAVA bytecode can be executed.
it's an implementation of the JVM which physically exists.
JVM, JRE, and JDK are platform-dependent. 
Java is platform-independent.

![jdk-jvm](https://user-images.githubusercontent.com/73180409/226957816-1b4fa937-0cf0-4c1a-a395-cd83f7d431c9.png)

## 3) JDK
JDK stands for Java Development Kit or sometimes it is also referred to as Java Standard Edition Development Kit. 
It is the tool necessary to compile and package Java programs.
JDK is a development environment to develop a wide range of applications such as desktop applications, web applications 

## 4) Features of Java or Java buzzwords

| Rank | Features      |
|-----:|---------------|
|     1|simple         |
|     2|Object-oriented|
|     3|portable       |
|     4|independent    |
|     5|secured        |
|     6|robust         |
|     7|simple         |
|     8|Architectural natural|
|     9|dynamic        |
|    10|High Performance|
|    11|Multithreaded  |
|    12|Distributed    |


- What happens at runtime? 
Class file -> class Loader-> byte code verified -> Interpreter -> Runtime -> hardware.

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

## 9)Java is not pure Object-Oriented:
The first reason is that the Object-oriented programming language should only have objects whereas java contains 8 primitive data types like char, boolean, byte, short, int, long, float, double which are not objects. These primitive data types can be used without the use of any object.

- cbbsilfd

### Object
we need an object for method calls

1. Real-time entity 
2. behavior 
3. identity
4. state


## 10) primitive data types &  Wrapper class

| Non-Primitive type | primitive data types | Wrapper class |
| 	:---:         |     :---:      |    :---: |
| Class   | boolean     | Boolean    |
| Object     | byte       | Byte      |
| Array   | char     | Character    |
| String     | float       | Float     |
| Interface   | int     | Integer    |
|     | long       |Long     |
|    | short   | Short    |
|      |double       | Double      |

+ Non-primitive data types:
These data types are not predefined in Java. They are created by programmers.

+ primitive data types:
Primitive types are predefined (already defined) in Java

+ Wrapper class:
The wrapper class in Java provides the mechanism to convert primitive into the object and object into primitive. 

## 11) Autoboxing and Unboxing
The automatic conversion of primitive into an object is known as autoboxing.
The automatic conversion of wrapper type into its corresponding primitive type is known as unboxing.
## Example 1 

	
```java

public class Example{  
public static void main(String args[]){  

byte b=1;  
short s=2;  
int i=3;  
long l=4;  
float f=5.0F;  
double d=6.0D;  
char c='a';  
boolean b2= true;  
  
// Autoboxing: Converting primitives into objects  
Byte byteobj=b;  
Short shortobj=s;  
Integer intobj=i;  
Long longobj=l;  
Float floatobj=f;  
Double doubleobj=d;  
Character charobj=c;  
Boolean boolobj=b2;  
  
System.out.println("Byte object is: "+byteobj);  
System.out.println("Short object is: "+shortobj);  
System.out.println("Integer object is: "+intobj);  
System.out.println("Long object is: "+longobj);  
System.out.println("Float object is: "+floatobj);  
System.out.println("Double object is: "+doubleobj);  
System.out.println("Character object is: "+charobj);  
System.out.println("Boolean object is: "+boolobj);  
  
// Unboxing: Converting Objects to Primitives  
byte bytevalue=byteobj;  
short shortvalue=shortobj;  
int intvalue=intobj;  
long longvalue=longobj;  
float floatvalue=floatobj;  
double doublevalue=doubleobj;  
char charvalue=charobj;  
boolean boolvalue=boolobj;  
  
System.out.println("byte value: "+bytevalue);  
System.out.println("short value: "+shortvalue);  
System.out.println("int value: "+intvalue);  
System.out.println("long value: "+longvalue);  
System.out.println("float value: "+floatvalue);  
System.out.println("double value: "+doublevalue);  
System.out.println("char value: "+charvalue);  
System.out.println("boolean value: "+boolvalue);  
	}
}  
```
## &- AND , |-OR , !-NOT
![image](https://github.com/TrickAndTrack/Core-Java/assets/73180409/dc55b4ce-3f28-4938-9e55-b082aa8874a9)

## Example 2

```java
public class ExampleTwo {
public static void main(String[] args)    {
 
        // Creating an Integer Object with custom value is 1
        Integer i = new Integer(1);
 
        // Unboxing the Object
        int j = i;
 
        // Print statements
        System.out.println("Value of i is:" + i);
        System.out.println("Value of j is: " + i1);
 
        // Autoboxing of character
        Character ch = 'a';
 
        // Auto-unboxing of Character
        char cha = ch;
 
        System.out.println("Value of ch is: " + ch);
        System.out.println(" Value of cha is: " + cha);
    }
}
```

## Example 3
```java
public class ExampleThree {
 public static void main(String[] args)  {
        List<Integer> alist = new ArrayList<Integer>();
 
        // Adding the int primitives type values
        // Autoboxing
        alist.add(1);
        alist.add(2);
        alist.add(5);
	
        System.out.println(" Printing the ArrayList: " + al);
    }

```
## Example 4

```java
public class ExampleThree {
 public static void main(String[] args)  {
       
        List<Integer> list = new ArrayList<Integer>();
 
        // Adding the int primitives type values by  converting them into Integer wrapper object
        for (int i = 0; i < 10; i++)
 
            System.out.println(list.add(Integer.valueOf(i)));
		
	List<Integer> listsecond = new ArrayList<Integer>();	
        for (int i = 0; i < 10; i++)
            listsecond.add(i);
 
         int sumOdd = sumOfOddNumber(list);
 
        System.out.println("Sum of odd numbers = "+ sumOdd);	
    }

```

# 12) typecasting 
Typecasting refers to the process of converting a value from one data type to another in programming languages. 
There are two types of typecasting: implicit and explicit. Implicit typecasting occurs automatically when one data type is converted to another without the need for explicit instructions from the programmer. Explicit typecasting, on the other hand, requires the programmer to explicitly convert one data type to another using special functions or syntax.

 here's an example of typecasting in Java:
 ```
 double x = 10.5;   // x is a double
int y = 5;         // y is an integer
int z = (int)x + y;   // typecast x to int and add it to y

System.out.println(z);   // Output: 15
```
We can also use explicit typecasting to convert a value from one data type to another
```
int a = 15;    // a is an integer
String b = Integer.toString(a);   // typecast a to a string

System.out.println(b);   // Output: "15"

```
# Static 

1) static keyword is class level keyword(directly access heap memory).
2) compile-time memory allocation.
3) keyword used for memory allocation.
4) and directly call without any object.

`static variables`: A static variable is shared by all instances of the class. It is created when the class is loaded into memory and exists until the program exits. static variables are often used to store constants or values that are common to all instances of the class.

`Non-static variables` :we cannot access in static block.(Instance variables)

`static methods`: A static method is a method that belongs to the class itself rather than to an instance of the class. It can be called without creating an object of the class. static methods are often used for utility methods or methods that operate on static variables. a static method can access static data members and can change their value of it.

`non-static method`: belong to object & memory allocated at the time of runtime. 

`static blocks`: A static block is a block of code that is executed when the class is loaded into memory. It can be used to initialize static variables or to perform any other actions that need to be done when the class is loaded.

```
public class MyClass {
    static int count;    // static variable
    
    static void incrementCount() {    // static method
        count++;
    }
    
    static {    // static block
        count = 0;
    }
}
```



Visit https://github.com	
