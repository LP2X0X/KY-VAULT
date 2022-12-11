The params keyword is useful when we do not know the number of arguments a method has. 
The parameter type must be a single-dimensional array.
```csharp
params <type>[] <name>
```

```csharp
// Note that no additional parameters are permitted after the params keyword in a method declaration, 
// and only one params keyword is permitted in a method declaration.
// Hence, the following method declaration is fine:  
public void PrintNames2(int a, double b, params int[] ages)  
// but the following declarations are not  
public void PrintNames3(int a, params string[] names, double b)
public void PrintNames4(params string[] names, params int[] ages)
```