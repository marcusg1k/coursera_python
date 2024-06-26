 python beginner notes

  First created by Guido Van Rossum in 1991. 
  -> py resources:   https://docs.python.org/3/ , python uses interpreter not a compiler. 
  Whenever there is a change to the syntax or semantics of the language, new major updates tend to release. 
  There are platform specific scripting languages, Powershell is used on windows and BASH is used on linux. 
  Functions = Pieces of code that perform a unit of work. (if, while, for)
  Keywords - Reserved words that are used to construct instructions. 
  using double quotations lets the intepreter know the text preceding is considered a string for example: "Hello, World" <- considered a string. Any text that isnt in quotations is considered part of the code. 
  General scripting languages like perl or ruby. 

  Math operands explained:
 x + y            Addition + operator returns the sum of x plus y
 x - y             Subtraction - operator returns the difference of x minus y
 x * y            Multiplication * operator returns the product of x times y
 x / y             Division / operator returns the quotient of x divided by y
 x**e            Exponent ** operator returns the result of raising x to the power of e 
 x**2            Square expression returns x squared
 x**3            Cube expression returns x cubed
 x**(1/2)    Square root (½) or (0.5) fractional exponent operator returns the square root of x
 x // y           Floor division operator returns the integer part of the integer division of x by y
 x % y          Modulo operator returns the remainder part of the integer division of x by y

   Key Terms
   Platform-specific / OS specific scripting language - Platform-specific scripting languages, like PowerShell (for Windows) and Bash (for Linux), are used by system administrators on those platforms. 
   Client-side scripting language - Client-side scripting languages, like JavaScript, are used mostly for web programming. The scripts are transferred from a web server to the end-user’s internet browser, then executed in the browser.
   Machine language - Machine language is the lowest-level computer language. It communicates directly with computing machines in binary code (ones and zeros). In binary code, one equals a pulse of electricity and zero equals no electrical pulse. Machine language instructions are made from translating languages like Python into complex patterns of ones and zeros. 
   Cross-platform language - Programming language that is compatible with one or more platforms / operating systems (e.g., Windows, Linux, Mac, iOS, Android).
   Object-oriented programming language - In object-oriented programming languages, most coding elements are considered to be objects with configurable properties. For example, a form field is an object that can be configured to accept only dates as input in the mm/dd/yy format, and can be configured to read from and write to a specific database. 
   Python interpreter - An interpreter is the program that reads and executes Python code by translating Python code into computer instructions.
  Python can also be used as a calculator for example (1+2) = 3. To get 2 to the power of 10 it is inputted by using (2**10) = 1024. 
  Values: True, False, None
  Conditions: if, elif, else
  Logical operators: and, or, not
  Loops: for, in, while, break, continue
  Functions: def, return  

  Glossary terms ~ course 1 module 1
  Automation: The process of replacing a manual step with one that happens automatically
  Client-side scripting language: Primarily for web programming; the scripts are transferred from a web server to the end-user’s internet browser, then executed in the browser
  Code editors: Tools to provide features, including syntax highlighting, automatic indentation, error checking, and autocompletion
  Computer program: A step-by-step list of instructions that a computer follows to reach an intended goal
  Functions: A reusable block of code that performs a specific task
  IDE: A software application that provides comprehensive facilities for software development
  Interpreter: The program that reads and executes code
  Input: Information that is provided to a program by the end user
  Logic errors: Errors in code that prevent it from running correctly
  Machine language: Lowest-level computer language. It communicates directly with computing machines in binary code (ones and zeros)
  Object-oriented programming language: Most coding elements are considered to be objects with configurable properties
  Output: the end result of a task performed by a function or computer program
  Platform-specific scripting language: Language used by system administrators on those specific platforms
  Programming: The process of writing a program to behave in different ways
  Programming code: A set of written computer instructions, guided by rules, using a computer programming language
  Programming languages: Language with syntax and semantics to write computer programs
  Python: A general purpose programming language
  Python interpreter: Program that reads and executes Python code by translating Python code into computer instructions
  Script: Often used to automate specific tasks
  Semantics: The intended meaning or effect of statements, or collections of words, in both human and computer languages
  Syntax: The rules for how each statement is constructed in both human and computer languages
  Variables: These are used to temporarily store changeable values in programming code

  Implicit Conversion: The interpreter automatically converts one data type into another
  Explicit Conversion: We manually convert the data type of one to incorporate use into another data type 
  str() - converts a value (often numeric) to a string data type
  int() - converts a value (usually a float) to an integer data type 
  float() - converts a value (usually an integer) to a float data type

  Dictionary: Stores key:value pairs, immutable keys but mutable and duplicate values (no, it is unordered and random)
  Set: An unordered collection of unique elements, mutable but unique elements only (no, it is unordered and unique)
  List: A sequential, mutable collection of any data type, mutable and allows duplicate elements (yes, and with numeric index assignment) 
  String: A sequential, immutable collection of textual data, immutable but allows duplicate elements (yes, but with a sequence of textual data) 
  Tuple: A sequential, immutable collection of any data type, immutable but allows duplicate elements (yes, and with numeric index assignment)

Dictionaries vs Lists: 
Both dictionaries and lists:
are used to organize elements into collections;
are used to initialize a new dictionary or list, use empty brackets;
can iterate through the items or elements in the collection; and
can use a variety of methods and operations to create and change the collections, like removing and inserting items or elements.

Dictionaries only:
are unordered sets;
have keys that can be a variety of data types, including strings, integers, floats, tuples;.
can access dictionary values by keys;
use square brackets inside curly brackets { [ ] };
use colons between the key and the value(s);
use commas to separate each key group and each value within a key group;
make it quicker and easier for a Python interpreter to find specific elements, as compared to a list.

Instance methods
Instance methods are the most common type of methods in Python. You define instance methods within a class by creating functions inside the class definition. When you instantiate instances of a class, those individual instances can have their methods called so the program can control and modify those instances directly. Instance methods can take a parameter called self, which represents the instance the method is being executed on, that allows you to access attributes of the instance using dot notation, like self.name, which will access the name attribute of that specific instance of the class object. When you have variables that contain different values for different instances, these are called instance variables.

Class methods
Class methods, on the other hand, are called for the class itself instead of an instance. They are marked with a @classmethod decorator and take a cls parameter that points to the class—and not any specific instance—when the method is called. One common use-case for class methods is to create and modify data structures that contain records for all instances of a class. Usually, programmers make a list inside the class definition, and methods to add instances of the class to that list in order to keep track of that class. 

Static methods
Lastly, static methods, marked with a @staticmethod decorator, do not take a self or a cls parameter. Static methods behave like plain functions, except that you can call them directly from the class. It is important to note that you do not have to actually instantiate the class, the methods just reside in there. This is because class definitions are themselves an object (i.e., an instance of abstract base class), which reduces overhead and allows functions to be encapsulated in an easy-to-use encapsulation. Programmers use static methods when the method does not need to access any instance or class-specific data.

sort vs sorted function: sorted returns a new list, while sort returns the same list reorganized



