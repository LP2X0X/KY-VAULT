- If you want to append data to an existing file, you create a StreamWriter instance like this:
```csharp
// True indicates that we want to append the data
StreamWriter sw = new StreamWriter(path, true);
// To override
StreamWriter sw = new StreamWriter(path);
```
- After we instantiate our StreamWriter object, we can start writing to our file using the WriteLine() method as shown below:  
```csharp
sw.WriteLine(“It is easy to write to a file.”);
```
