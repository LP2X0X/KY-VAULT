- Property Element Syntax is an alternative syntax used for providing values for complex types.
- Instead of the property being specified as an attribute within the element tag, the property is specified using an opening element tag in _elementTypeName_._propertyName_ form, the value of the property is specified within, and then the property element is closed.
- Specifically, the syntax begins with a left angle bracket (<), followed immediately by the type name of the class or structure that the property element syntax is contained within. This is followed immediately by a single dot (.), then by the name of a property, then by a right angle bracket (>).
- The child element is referred to as a *property element*.
### Example
```csharp
<Button>  
	<Button.Background>  
		<SolidColorBrush Color=”Blue” />  
	</Button.Background>  
</Button>
```