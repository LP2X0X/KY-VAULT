![[Pasted image 20221216195318.png|center]]
# HorizontalAlignment Property
- The HorizontalAlignment property declares the horizontal alignment characteristics to apply to child elements. The following table shows each of the possible values of the HorizontalAlignment property.

| Member            | Description                                                                                                                         |
| ----------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
| Left              | Child elements are aligned to the left of the parent element's allocated layout space.                                              |
| Center            | Child elements are aligned to the center of the parent element's allocated layout space.                                            |
| Right             | Child elements are aligned to the right of the parent element's allocated layout space.                                             |
| Stretch (Default) | Child elements are stretched to fill the parent element's allocated layout space. Explicit Width and Height values take precedence. |

![[layout-horizontal-alignment-graphic.png|center]]

# VerticalAlignment Property
- The VerticalAlignment property describes the vertical alignment characteristics to apply to child elements. The following table shows each of the possible values for the VerticalAlignment property.

| Member            | Description                                                                                                                         |
| ----------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
| Top               | Child elements are aligned to the top of the parent element's allocated layout space.                                               |
| Center            | Child elements are aligned to the center of the parent element's allocated layout space.                                            |
| Bottom            | Child elements are aligned to the bottom of the parent element's allocated layout space.                                            |
| Stretch (Default) | Child elements are stretched to fill the parent element's allocated layout space. Explicit Width and Height values take precedence. |

![[layout-vertical-alignment-graphic.png|center]]

# Margin Properties
- The Margin property describes the distance between an element and its child or peers. Margin values can be uniform, by using syntax like Margin="20". With this syntax, a uniform Margin of 20 device independent pixels would be applied to the element. 
- Margin values can also take the form of four distinct values, each value describing a distinct margin to apply to the **left, top, right, and bottom** (in that order), like Margin="0,10,5,25". 
- Proper use of the Margin property enables very fine control of an element's rendering position and the rendering position of its neighbor elements and children.
```ad-note
A non-zero margin applies space outside the element's ActualWidth and ActualHeight.
```

# Padding Property
- Padding is similar to Margin in most respects. The Padding property is exposed on only on a few classes, primarily as a convenience: Block, Border, Control, and TextBlock are samples of classes that expose a Padding property. The Padding property enlarges the effective size of a child element by the specified Thickness value.
# Different between Margin and Padding
- In the Windows UI world, **Margin** is a property of the FrameworkElement class, whereas **Padding** is a Control and Border class property. So, for all Control- and Border- derived classes, both these properties are present and have the following behavior:  
  - **Margin** represents the distance between one side of a User Interface (UI) element and the adjacent UI element or the container's limit. For instance, the distance between a TextBox and a Button to its right will be the TextBox's right margin width + the Button's left margin width.  
  - **Padding** represents the distance between the side of the control (which can be the margin) and its content. The content depends on the type of the control.  
  - Margin is outside the UI element, while Padding is inside it.