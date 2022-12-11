- An enum (which stands for enumerated type) is a special data type that allows programmers to provide meaningful names for a set of integral constants.
- To declare an enum, we use the enum keyword followed by the name of the enum.
- By default, each member in the enum is assigned an integer value, starting from zero.
- There are two main reasons for using enums:
	- The first is to improve the readability of your code.
	- The second reason is to restrict the values that a variable can take.
### Example
```csharp
enum DaysOfWeek
{
Sun, Mon, Tues, Wed, Thurs, Fri, Sat
}
```

```ad-note
Note that we do not put a semi-colon at the end of the last member.
```

- After declaring the DaysOfWeek enum, we can declare and initialize a DaysOfWeek variable like this:
```csharp
DaysOfWeek myDays = DaysOfWeek.Mon;
```

- If you want to assign a different set of integers to your enum members, you can do the following:
```csharp
enum DaysOfWeekTwo  
{  
Sun = 5, Mon = 10, Tues, Wed, Thurs, Fri, Sat  
}
// So Console.WriteLine((int)Sun) will return 5
```
- As we did not assign values for Tues to Sat, consecutive numbers after 10 will be assigned to them. That is Tues = 11, Wed = 12 and so on.
- If you want to change the underlying data type from int to another data type, you add a colon after the enum name, followed by the desired data type.
```csharp
enum DaysOfWeekThree : byte
{  
Sun, Mon, Tues, Wed, Thurs, Fri, Sat  
}
```