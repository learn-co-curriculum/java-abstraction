# Abstraction

## Learning Goals

- Discuss abstraction in object-oriented programming
- Compare abstract classes and interfaces

## Introduction


A programmer uses abstraction to hide all but the essential details about an object in an effort
to reduce complexity and increase adaptability.  Abstraction give us the ability to separate **what** should
happen from **how** it should happen.

Abstraction can be achieved in Java by defining interfaces and abstract classes,
along with their concrete class implementations.


## Comparing Abstract Classes and Interfaces

| Abstract Class                                                                                | Interface                                                                                               |
|-----------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------|
| May define instance and static variables                                                      | May define constant variables (static+final). Instance and non-final static variables are not allowed.  |
| Can't instantiate using `new` operator.                                                       | Can't instantiate using `new` operator.                                                                 |
| Can define parameterized constructors. Always has a default constructor.                      | Can't define a constructors.  Does not have a default constructor.                                      | 
| Can't instantiate using `new` operator.                                                       | Can't instantiate using `new` operator.                                                                 |
| May define any number of concrete or abstract methods, including instance and static methods. | May define any number of abstract, default, or static methods.                                          |

An abstract class is useful when we want to define a base class that declares the
generalized structure and behavior of a given abstraction without providing a complete implementation of every method.
Each subclass will fill in the details.

An interface is useful when object functionalities are defined as a contract, i.e. a set of abstract methods,
without concern about who implements the required behavior.

When to use an abstract class versus an interface?  An abstract class is appropriate when describing what something is,
while an interface describes what something can do.  For example, a dog is an animal (`Animal` is an abstract class),
while a duck can swim (`Swimmable` is an interface).

