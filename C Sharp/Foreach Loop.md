- A foreach loop is very useful if you want to get information from an array or list, without making any changes to it.
- Suppose you have:
```csharp
char[] message = { ‘H’, ‘e’, ‘l’, ‘l’, ‘o’ };  
```
- You can use the following code to display the elements of the array: 
```csharp
foreach (char i in message)  
Console.Write(i);
```
