# Declarative UI
- WPF allows you to construct your interface using a markup language called [[WPF/XAML/XAML]] (pronounced *zammel*, rhymes with camel). XAML is a much richer markup language than HTML, and it has less ambiguity. Visual Studio, as well as some members of the Expression family of products are able to generate XAML natively.
# Intelligent Layout
- WPF provides an extensible layout system for visually arranging the elements of a user interface. It can intelligently resize and adjust, depending on how you define the layout.
# Scalable Graphics  
- Graphics in WPF are [[Vector Graphic|vector based]], in contrast to [[Raster Graphic|raster based]]. Vector graphics are inherently scalable and typically require less storage than a comparable raster image.
- WPF still has plenty of support for raster graphics, but vectors are an excellent fit for constructing user interfaces.
# Templates
- WPF makes it very easy to create reusable elements for your user interfaces. There are two types of templates in WPF: control templates and data templates. 
	- Control templates enable you to redefine the way a control looks.
	- Data templates are similar, except that instead of defining the way a control looks, they define the way certain types of data are rendered.
# [[Data Binding|Binding]]
# Styling
- WPF really shines when it comes to making an application look pretty. WPF styles are richer and have less ambiguity. They encompass all the visual characteristics you would expect, such as padding, margin, position, color, and so on. But you can also use styles to declare nonvisual properties.
- Styles are also easy to reuse, and when you combine them with templates, you are able to do some amazing things.
# Triggers  
- Both templates and styles in WPF support the notion of triggers. A trigger enables you to tell WPF something like this: “When the mouse is over the button, make the background purple.” In other words, triggers enable you to declaratively handle changes of state. You will also find them useful for kicking off animations.
# Animation  
- The animation framework in WPF is very impressive, and a great deal more useful than you might think. Most properties in WPF can be animated, and support exists for timelines, key frames, and interpolation. Animations are easily integrated with templates and styles.
# 3D 
- Finally, WPF allows for some basic 3D modeling and animation. I say basic because WPF is not intended for building high-performance 3D applications. Nevertheless, the 3D features are powerful and easily integrated into any user interface.
