- A List stores values like an array, but elements can be added or removed at will.
# Declaration and Initialization
- To declare a list of integers, we write:
```csharp
List<int> userAgeList = new List<int>();
```
- You can choose to initialize the list at the point of declaration like this:
```csharp
List<int> userAgeList = new List<int> {11, 21, 31, 41};
```
# Notable Properties and Methods
- You can add members to a list using the *Add()* method.
- To find out the number of elements in the list, use the *Count* **property**.
- To add members at a specific position, use the *Insert()* method.
```csharp
userAgeList.Insert(<index>, <value>);
```
- To remove members from the list, use the *Remove()* method. The Remove() method takes in one argument, which is the value, and removes the first occurrence of that argument.
- To remove a member at a specific location, use the *RemoveAt()* method.
- To check if a list contains a certain member, use the *Contains()* method.
- To remove all items in a list, use the *Clear()* method.