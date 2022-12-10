# About
- Profile diagram, a kind of structural diagram in the Unified Modeling Language (UML), provides a generic extension mechanism for customizing UML models for particular domains and platforms.
# When to Use Profile Diagram
- Creation of a new metamodel.
- Extension and modification of the UML metamodel.
- Extension of the UML metamodel with language-inherent mechanisms.
# Basic Concepts of Profile Diagram
## Stereotypes
- Stereotypes allow you to increase vocabulary of UML. You can add, create new model elements, derived from existing ones but that have specific properties that are suitable to your problem domain. 
- Stereotypes are used to introduce new building blocks that speak the language of your domain and look primitive. It allows you to introduce new graphical symbols.
- For example: When modeling a network you might need to have symbols for << router >>, << switches >>, << hub >> etc. A stereotype allows you to make these things appear as primitive.
![[01-class-with-stereotype.png|center]]
## Tagged Values
- Tagged values are used to extend the properties of UML so that you can add additional information in the specification of a model element. It allows you to specify keyword value pairs of a model where keywords are the attributes. 
- Tagged values are graphically rendered as string enclose in brackets.
![[02-class-with-tagged-value.png|center]]
## Constraints
- They are the properties for specifying semantics or conditions that must be held true at all the time. 
- It allows you to extend the semantics of UML building block by adding new protocols. Graphically a constraint is rendered as string enclose in brackets placed near associated element.
![[03-constraint.png|center]]