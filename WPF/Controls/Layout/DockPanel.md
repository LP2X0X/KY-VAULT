- DockPanel defines an area within which you can arrange child elements either horizontally or vertically, relative to each other.
- The DockPanel makes it easy to dock content in all four directions (top, bottom, left and right). This makes it a great choice in many situations, where you want to divide the window into specific areas, especially because by default, the last element inside the DockPanel, unless this feature is specifically disabled, will automatically fill the rest of the space (center).
### Example
```csharp
<Window x:Class="WpfTutorialSamples.Panels.DockPanel"
        xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"
        xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml"
        Title="DockPanel" Height="250" Width="250">
	<DockPanel>
		<Button DockPanel.Dock="Left">Left</Button>
		<Button DockPanel.Dock="Top">Top</Button>
		<Button DockPanel.Dock="Right">Right</Button>
		<Button DockPanel.Dock="Bottom">Bottom</Button>
		<Button>Center</Button>
	</DockPanel>
</Window>
```
![[dockpanel_simple.png|center]]

```ad-note
As already mentioned, we don't assign a dock position for the last child, because it automatically centers the control, allowing it to fill the remaining space. You will also notice that the controls around the center only takes up the amount of space that they need - everything else is left for the center position. That is also why you will see the Right button take up a bit more space than the Left button - the extra character in the text simply requires more pixels.
The last thing that you will likely notice, is how the space is divided. For instance, the Top button doesn't get all of the top space, because the Left button takes a part of it. The DockPanel decides which control to favor by looking at their position in the markup. In this case, the Left button gets precedence because it's placed first in the markup. Fortunately, this also means that it's very easy to change, as we'll see in the next example, where we have also evened out the space a bit by assigning widths/heights to the child controls.
```

```csharp
<Window x:Class="WpfTutorialSamples.Panels.DockPanel"
        xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"
        xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml"
        Title="DockPanel" Height="250" Width="250">
	<DockPanel>
		<Button DockPanel.Dock="Top" Height="50">Top</Button>
		<Button DockPanel.Dock="Bottom" Height="50">Bottom</Button>
		<Button DockPanel.Dock="Left" Width="50">Left</Button>
		<Button DockPanel.Dock="Right" Width="50">Right</Button>	
		<Button>Center</Button>
	</DockPanel>
</Window>
```
![[dockpanel_widths_heights.png|center]]

```ad-note
As already mentioned, the default behavior is that the last child of the DockPanel takes up the rest of the space, but this can be disabled using the **LastChildFill**.
```