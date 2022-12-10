# About
- Component diagrams provide a simplified, high-order view of a large system.
- Classifying groups of classes into components supports the interchangeability and reuse of code.
- Components are considered autonomous, encapsulated units within a system or subsystem that provide one or more interfaces.
# Component Diagram Notations
## 1.Component
- A component is drawn as a rectangle with optional compartments stacked vertically.
- A component can be represented as just a rectangle with the component's name and the component stereotype text and/or icon.
- The component stereotype's text is "component" and the component stereotype icon is a rectangle with two smaller rectangles protruding on its left side.
![[02-uml-component-symbol 1.webp||center]]
## 2.Component Interfaces
- **Provide Interface**: Provided interfaces define "a set of public attributes and operations that must be provided by the classes that implement a given interface".
- **Required Interface**: Required interfaces define "a set of public attributes and operations that are required by the classes that depend upon a given interface".
![[03-provided-and-required-interface.webp|center]]
## 3.Component Assemblies
- Components can be "wired" together using to form subsystems, with the use of a ball-and-socket joint.
![[04-component-diagram-ball-and-socket-joint.webp|center]]
## 4.Port
- A port (definition) indicates that the component itself does not provide the required interfaces (e.g., required or provided). Instead, the component delegates the interface(s) to an internal class.
![[05-component-diagram-port.webp|center]]
# Types of relationship
## 1.Association
- Relationship between typed instances.
- They are represented by a **solid line** between classes.
![[Pasted image 20221208133923.png|center]]
## 2.Composition
- Composition aggregation requires a part instance to be included in at most one composition at a time.
- If a composite is deleted, all its parts are usually deleted with it.
![[Pasted image 20221208134214.png|center]]
## 3.Aggregation
- The child component can exist on its own even without being a part of the class.
![[Pasted image 20221208134317.png|center]]
## 4.Constraint
- A condition or restriction expressed as a text in a natural language or in a machine-readable language.
![[Pasted image 20221208134519.png|center]]
## 5.Dependency
- Dependency is a relationship, where an element or set of elements require other elements for their specification or implementation.
![[Pasted image 20221208134652.png|center]]
## Inheritance
- Is a taxonomic relationship between a more general classifier and a more specific classifier.
![[Pasted image 20221208134804.png|center]]