- Markup Extensions are a XAML technique for obtaining a value that's not a primitive or a specific XAML type.
- Markup extensions are identified by the presence of curly brackets ({}). The first word in the markup extension tells WPF what kind of extension it is. The name of the extension is optionally followed by a set of named parameters. 
### Example
- Suppose we have a specific color we want to use as the background for  several buttons in a WPF application. We could set the Background property on each of the buttons to use the same color, but it would become tedious if we ever needed to change that color. With WPF, we can store the color with a lookup key in an application’s resources. Now we can set the background of the buttons to the color we stored in the resources. If we want to change the color, we need do so in only one place. That’s a lovely scenario, but how would we handle this in XAML?
```csharp
<Button Background=”{StaticResource ResourceKey=myColor}”  
Content=”Click Me” />
```
- Many extensions have a default parameter. You don’t have to explicitly reference a default parameter. You are allowed to omit the parameter name and the equal sign.
```csharp
<Button Background=”{StaticResource myColor}”  
Content=”Click Me” />
```
- In some cases, you will have more than one parameter. If you do, you must separate name/value pairs with commas.
```csharp
{ExtensionName Param1=Value1, Param2=Value2, Param3=Value3}
```