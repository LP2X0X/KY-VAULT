# Notable Properties and Methods
- The *Substring()* **method** is used to extract a substring from a longer string. It requires two arguments. 
	- The first tells the compiler the index of the starting position to extract.
	- The second tells the compiler the length.
- We can use the *Equals()* **method** to compare if two strings are identical.
- The *Split()* **method** splits a string into substrings based on an array of user-defined separators. After splitting the string, the Split() method returns an **array** that contains the resulting substrings. (Reference: https://learn.microsoft.com/en-us/dotnet/api/system.string.split?view=net-7.0)
# String Format
1. Using *Placeholders*, if we write:
```csharp
Console.WriteLine(“{0}! You scored {1} marks for your test.”, "Good morning”, results);
```
- We will get: 
```csharp
Good morning! You scored 79 marks for your test.
```
2. We can specify how we want numeric values to be displayed when using placeholders. This is done using a *Format Specifier*, such as the C and F specifiers.
```csharp
Console.WriteLine(“The number is {0:F3}.”, 123.45678);
```
- We will get: 
```csharp
The number is 123.457.
```
- The C specifier is for formatting currencies; it adds the “$” symbol in front of the number and displays the number with 2 decimal places. In addition, it separates every thousand with a comma.
