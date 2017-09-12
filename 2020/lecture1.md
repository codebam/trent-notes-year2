# Lecture 1 - 2020

## C# Object-Oriented Prog.

1. Class
    - data members
        - typically private
        - how something is represented
    - methods
        - typically public
        - the behavior
2. Inheritence
    - B is an instance of A
3. Polymorphism
    - sometimes referred to as dynamic binding
4. Composition (interfaces)
    - B has A

#### Static vs Non-static (instance)

- static: a method you cannot create objects from
- static data member
    - is a data member that belongs to the class
- static class
    - all of it's data members have to be static
    - you can't create an instance of a static class

Example:
``` csharp
Animal a;
a = new Animal(..);
```

- all objects are reference types
- everything is either a reference type of a value type
- value type
    - int
    - float
    - char
    - bool
    - ...

- virtual allows the child to override

``` csharp
public virtual void M() {} // parent
public override void M() {} // child
```

- at the  very top is class object
- everything derives from the object class

- Methods in the object class
    - Equals
    - Finalize
    - GetHashCode
    - GetType
    - MemberwiseClone
    - ReferenceEquals
    - ToString

- abstract
    - has no body
    - can't create an object from an abstract class
    - you inherit from it and write the method
    - interfaces are always abstract and are all public
