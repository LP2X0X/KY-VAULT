- Interfaces are much like abstract classes in that they cannot be instantiated and must be inherited. However, interfaces are more conceptual than abstract classes. They can only contain methods with no bodies. In addition, they cannot contain fields but can contain properties. Interfaces also cannot have static members. When a child class inherits an interface, we say that it implements the interface.
```ad-note
One of the key differences between an abstract class and an interface is that **a class** can only inherit **one abstract class** but can implement **multiple interfaces**.
```

```ad-note
It is considered good practice to start with the letter "I" at the beginning of an interface, as it makes it easier for yourself and others to remember that it is an interface and not a class.
```

### Example
```csharp
// Interface
interface IAnimal 
{
  void animalSound(); // interface method (does not have a body)
}

// Pig "implements" the IAnimal interface
class Pig : IAnimal 
{
  public void animalSound() 
  {
    // The body of animalSound() is provided here
    Console.WriteLine("The pig says: wee wee");
  }
}

class Program 
{
  static void Main(string[] args) 
  {
    Pig myPig = new Pig();  // Create a Pig object
    myPig.animalSound();
  }
}
```