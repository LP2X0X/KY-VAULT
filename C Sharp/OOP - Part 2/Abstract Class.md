- An abstract class is a special type of class that is created strictly to be a base class for other classes to derive from. They cannot be instantiated.
- Abstract classes may have fields, properties and methods just like any other classes. However, they cannot have static members.
- In addition, abstract classes can have a special type of method known as abstract methods. Abstract methods are methods that have no body and MUST be implemented in the derived class. They can only exist in abstract classes.
---
- To declare an abstract class, simply add the abstract keyword before the keyword class:
```csharp
abstract class MyClass
```
- To declare an abstract method inside an abstract class, add the abstract keyword before the return type:
```csharp
public abstract void MyAbstractMethod();
```
- To implement an abstract method in the derived class, we use the override keyword:
```csharp
public override void MyAbstractMethod()
```
