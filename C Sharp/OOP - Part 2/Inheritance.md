- Inheritance is one of the key concepts of object-oriented programming.
- Simply stated, inheritance allows us to create a new class from an existing class so that we can effectively reuse existing code.
- The class whose members are inherited is called the *base class*, and the class that inherits those members is called the *derived class*. A derived class can have only one direct base class. Conceptually, a derived class is a **specialization** of the base class.
- When you define a class to derive from another class, the derived class implicitly gains all the members of the base class, except for its constructors and finalizers.
- We indicate that a child class is derived from the parent class using a colon (:) like this:
```csharp
class <child class> : <parent class>
```

```ad-note
Whenever we create a child object, the parent class constructor with the same [[Signature - Definition|signature]] is always called first.
```

- The other way to declare a child constructor is to use the colon sign (:) and the base keyword to call a non-parameter-less constructor in the parent class.
```csharp
public <constructor name>(<parameters>) : base (<parameters of base class>)
```