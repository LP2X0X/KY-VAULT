# About
- Package Diagram shows the arrangement and organization of model elements in middle to large scale project.
- Package diagram can show both structure and dependencies between sub-systems or modules, showing different views of a system and so on.
# Purpose of Package Diagrams
- Package diagrams are used to structure high level system elements. Packages are used for organizing large system which contains diagrams, documents and other key deliverables.
	- Package Diagram can be used to simplify complex class diagrams, it can group classes into packages.
	- A package is a collection of logically related UML elements.
	- Packages are depicted as file folders and can be used on any of the UML diagrams.
# Building Blocks
## Package
- Packages appear as rectangles with small tabs at the top.
- The package name is on the tab or inside the rectangle.
- The dotted arrows are dependencies.
- One package depends on another if changes in the other could possibly force changes in the first.
## Stereotype
- Stereotype is a high-level classification of an object that gives some idea of what the object is.
- Classes can be grouped by stereotypes, whose names are written between the angle brackets (<< >>) above the class name.
- Stereotype allows us to extend UML to fit our modeling needs more specifically.
- Stereotyping a UML element makes it act as something that has a specific properties.
## Dependency Notation
- << import >> - one package imports the functionality of other package.
- << access >> - one package requires help from functions of other package. 