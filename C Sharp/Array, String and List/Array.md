# Declaration and Initialization
- An array can be <u>declared</u> and <u>initialized</u> as follows:
	- int indicates that this variable stores int values.
	- [] indicates that the variable is an array instead of a normal variable.
	- userAge is the name of the array.
	- {21, 22, 23, 24, 25} are the five integers that the array stores.
```csharp
int[] userAge = {21, 22, 23, 24, 25};
```
- We can declare an array first and initialize it later using the *new* **operator**.
```csharp
int[] userAge = new int[5];  
userAge = new [] {21, 22, 23, 24, 25};
```
---
# Notable Properties and Methods
- The *Length* **property** of an array tells us the number of items the array has.
- The *Copy()* **method** allows you to copy the contents of one array into another array, starting from the first element.
	```csharp
	Array.Copy(<source>, <dest>, <num_of_elem>);
	```
- The *Sort()* **method** allows us to sort our arrays.
- We use the *IndexOf()* method to determine if a certain value exists in an array. 
	- If it exists, the method returns the index of the first occurrence of that value. 
	- If it does not exist, the method returns -1.