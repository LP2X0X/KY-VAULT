```ad-note
Remember, an object created by a class has the < class > **type**.
```
- The GetType() method returns the runtime type of an object.  
- The typeof() method takes the name of a data type (e.g. int, float, or the name of a class) and returns the type of that name, which we can then compare with the result of the GetType() method on the left.
## Example
```csharp
if (<object>.GetType() == typeof(<object>))
```