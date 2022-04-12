# Design Patterns

Design patterns are reusable solutions to common programming problems.

---

There are three mayor categories to divide them:

## Creational Patterns

- Deal with the creation (construction) of objects
- Explicit (constructor) vs. Implicit (dependency injection, reflection, etc)
- Wholesale (single statement) vs. piecewise (step-by-step)

**Types:**

- Builder
- Factories
  - Abstract Factory
  - Factory Method
- Prototype
- Singleton



## Structural Patterns

- Concerned with the structure (e.g., class members)
- Many patterns are wrappers that mimic the underlying class interface
- Stress the importance of good API design

**Types**:

- Adapter
- Bridge
- Composite
- Decorator
- Facade
- Flyweight
- Proxy



## Behavioral Patterns

- They are all different, no central theme

**Types:**

- Chain of Responsibility
- Command
- Interpreter
- Iterator
- Mediator
- Memento
- State
- Strategy
- Template Method
- Visitor

---

## SOLID Design Principles

**Single Responsibility**

The principal idea is that you have to think about the classes and functions to do a couple of related things. The anti pattern of this could be called a God Class, which is the one who does a lot of things, becoming very difficult to read or refactor.

Separation of concerns is another related things, you have to analyze and separate methods and functions by how much they are related by what they do.

**Open-Closed**

This means that classes are open for extension but closed for modification. Instead of adding new methods to existent classes, you make new classes to satisfy new necessities.

**Liskov Substitution**

This defines that objects of a superclass shall be replaceable with objects of it's subclasses without breaking the application. The objects of the subclasses should behave in the same way as the objects of the superclass.

The overridden methods of a subclass needs to accept the same input parameters values as the method of the superclass.

It's hard to implement, but we can follow these two rules:

- Don't implement an stricter validation rules on input parameters than implemented by the parent class.
- Apply at least the same rules to all output parameters as applied by the parent class.

**Interface Segregation**

It's a way to take away some methods that other classes may not use, but you will have to define anyway because the parent class declares it.

This makes you to identify which methods may not be usable for every subclasses and segregate them apart so other extended subclasses stay clear and free of surprises to other developers.

**Dependency Inversion**

Basically, design your classes so the high-level modules never depend or know the implementation details of the low-level modules.

In a low-level module, we can develop all the implementation details of accessing to some data. So we can provide to the high-level module an abstracted and detail-free way to access the information results.

---

## Creational Patterns

**Builder**
