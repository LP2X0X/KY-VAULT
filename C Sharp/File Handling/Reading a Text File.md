- To read data from a text file, we use the StreamReader class.
### Example
- Suppose we want to read data from the file “myFile.txt” located on the C drive. The example below shows how to do it.
```csharp
using System.IO
string path = “c:\\myFile.txt”;
try
{
	using (StreamReader sr = new StreamReader(path))  
	{  
		// While loop to read the text file line by line
		while (sr.EndOfStream != true)  
		{  
			Console.WriteLine(sr.ReadLine());  
		}
		sr.Close();
	}
}
catch (FileNotFoundException e)
{
	Console.WriteLine(e.Message);
}

```
