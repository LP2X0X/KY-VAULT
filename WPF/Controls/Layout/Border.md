- A Border control is used to draw a border that surrounds its child control. Border is a single child element.
- The rendering of the border is quite flexible with options to control the positioning and thickness of the lines and whether the corners are right angled or curved.
### Example
```csharp
<Window x:Class="BorderDemo.MainWindow"
        xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"
        xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml"
        Title="Border Demo"
        Width="250"
        Height="200">
<StackPanel>
    <Border Margin="20"
            BorderBrush="DarkGreen"
            BorderThickness="5"
            Background="GreenYellow">
        <Label>Hello, world!</Label>
    </Border>
</StackPanel>
</Window>
```
![[Pasted image 20230109093118.png|center]]