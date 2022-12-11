A Property is commonly used to provide access to a private field in cases where the field is needed by other classes.
A Property contains two special methods known as accessors. The first accessor is a getter and the second is a setter:
	- The basic getter simply returns the value of the private field.
	- The setter sets the value of the private field.
By default, getter and setter have the same access level as the property itself. You can declare the setter as any [[Access Modifier|access modifier]].

```csharp
<Access Modifier> <Type> <Name>
{
	get
	{
	}
	set
	{
	}
}
```

```ad-note
Note that in cases where no additional logic is required in the getter and setter, C# provides us with a shorthand to declare the property. This is known as an *Auto-implemented Property*.
```csharp
<Access Modifier> <Type> <Name> { get; set; }
```

### Example
```csharp
private int hWorked;.  
public int HoursWorked  
{  
	get  
	{  
	return hWorked;  
	}  
	set  
	{  
	if (value > 0)  
		hWorked = value;  
	else  
		hWorked = 0;  
	}  
}
```

```ad-note
*value* is a keyword when it used inside a setter. It refers to the value that is on the right side of the assignment statement when users use the *property* to set the value of the private field.
```