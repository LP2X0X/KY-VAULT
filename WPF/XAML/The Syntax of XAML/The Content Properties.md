- Content is a special property. XAML specifies a language feature whereby a class can designate exactly one of its properties to be the XAML content property. The convention of setting the Content property implicitly is almost universally adopted.
- You can set the Content property implicitly using a child element.
### Example
```csharp
<Button Content=”Click Me” />
<Button>Click Me</Button>
```
