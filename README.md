# MyJavaCodingStyleCoding:
**Coding:**

Favor readability - if there's an ambiguous and unambiguous route, always favor unambiguous

Favor immutability

Do not perform bitwise and arithmetic operations on the same data

Do not use a null in a case where an object is required

Do not use deprecated or obsolete classes or methods

Classes that define an equals() method must also define a hashCode() method

Do not modify the underlying collection when an iteration is in progress

Initialize (almost) all local variables

Convert integers to floating point for floating-point operations

Variables should be declared in the innermost block that encloses all uses of the variable.

Don't Ignore Exceptions, Don't Catch Generic Exception

Do not attempt to help the garbage collector by setting local reference variables to null

Do not store unencrypted sensitive information on the client side

Do not serialize direct handles to system resources

Strive for logical completeness


**Naming:**

Treat acronyms as words (XmlHttpRequest > XMLHTTPRequest)

Class names should be nouns, in mixed case with the first letter of each internal word capitalized. Try to keep your class names simple and descriptive.

Interface names should be capitalized like class names.

Methods should be verbs, camel case.

The names of variables declared class constants and of ANSI constants should be all uppercase with words separated by underscores (“_”)

One-character variable names should be avoided except for temporary “throwaway” variables.


**Ordering:**

2.2.10 Class member ordering
	1.	Constants
	2.	Fields
	3.	Constructors
	4.	Override methods and callbacks (public or private)
	5.	Public methods
	6.	Private methods
	7.	Inner classes or interfaces


Parameter ordering in methods:

// Context always goes first
public User loadUser(Context context, int userId);

// Callbacks always go last
public void loadUserAsync(Context context, int userId, UserCallback callback);


**Misc:**

Use TODO comments for code that is temporary, a short-term solution, or good-enough but not perfect.

Remove dead code

Code lines should not exceed 100 characters.

When multiple methods are chained in the same line - for example when using Builders - every call to a method should go in its own line, breaking the line before the .

Each line should contain at most one statement. One declaration per line is recommended since it encourages commenting

No space between a method name and the parenthesis
