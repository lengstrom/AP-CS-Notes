##Software Development Lifecycle
###Waterfall model
Analysis of specification -> Program design -> Implementation -> Testing and Debugging -> Maintainence

**Specification**: written description of the project<br>
**Program Design**: fairly detailed plan for solving specification <br>
**Implementation**: code stuff
**Testing and debugging**: Plug in test data for each part of the domain + end / beginning / out of range values (extremes) and look for errors....

#####Types of errors
- Compile time error: Occurs during compilation, could be something like mismatching types or mispelling a keyword
- Run-time error: Occurs during execution, could be smething like dividing by 0 or accessing an array outside of its bounds
- Intent / logic error = one that fails to carry out the specification but whose syntax works fine.

**Robustness**: Write a program that won't...

- Give innacurate answers (ever)
- Crash if input data is invalid
- Allow execution to proceed if invalid data is entered

**Program Maintenance**: Clear / concise docs for newcomers / for you to modify the program as you see fit later on.

## Object Oriented Program Design
### Steps

- Identify classes to be written
- Identify behaviors for each class
- Determine relationships between classes
	- Inheritance - classes with common behavior
	- Composition - classes that contain eachother
- Write the interface (public method headers) for each class
- Implement the methods

### UML Diagrams

- Classes = rectangles
- French bracket quote things are used to hold the words "abstract" or "interface" to indicate the type of object that the rectangle represents
- Subclass <-> superclass relationship represented by line with unfilled heads (white fill)
- Classes that contain other classes use an arrow from the container class to the class being contained with a solid head (black fill)
- Class <-> interface relationship shown by dotted arrow with unfilled heads (white fill)


### Bottom up Development

- For each method, list all other classes that are needed to implement the method 
	- These classes are called collaborators
	- Classes that do not depend on other classes are known to be "independent"
- A *bottom up* approach is when individual classes are fully implemented and tested before being incorporated into the overall project
	- Constructors, then methods, should be added and tested once at a time
	- Barebones -> more features are added

### Top Down Development

- Programmer starts with an overview of the program and works down from the classes that control everything to the things that are controlled

### Implementing methods
- Procedural abstraction: Use helper methods within classes for procedures that are used multiple times to make sure that code doesn't have to be constantly rewritten
- Information hiding: ivars + helper methods (generally declared as private) prevent client classes from utilizing them
- Stub Method: Dummy method that stands in for another method until the actual one has been written... used to aid in the development of other methods / classes / interactions
- Algorithm: Code that solves a problem or achieves a goal

### Program Analaysis
- Assertions: precise statements about a program at any given point
	- The **precondition** for any piece of code is a statement about what is true immediately before the execution of the code.
	- The **postcondition** for a piece of code is a statement of what is true immediately after execution of that code.
- Efficiency: An efficient algorithm is economical in the use of...
	- **CPU time** (# of machine operations required to carry out the algo)
	- **Memory** (# and complexity of the variables that are used)
	
*A complete vocabulary list is [here](http://quizlet.com/21971923/ap-computer-science-program-design-and-analysis-vocabulary-flash-cards/). (I just found this on the internet, this is not my account / my set).*