## Object-Oriented Tenets

- the derived (child) class inherits the behavior of the parent class
- the child is typically a more special variant of the parent

polymorphism
``` csharp
            A
      -------------
      |     |     |
      B     C     D

A a;
B b;
a = b;
```

you can assign an instance of B to A, you can assign up the hierarchy

``` csharp
a.Print()
```
B, C, and D will inherit the Print method.
They can also override the method.

You cannot assign down the hierarchy without casting.
``` csharp
b = a; // can't do this
b = (B) a; // must cast
```

## Namespaces

``` csharp
namespace Numbers
{
    public class Fraction
    { ... }
    
    internal class Complex
    { ... }
    ...
}
```
