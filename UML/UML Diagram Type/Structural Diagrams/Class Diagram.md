# About
- Central modeling technique.
- Used in almost all object oriented methods.
- Describes types of objects in the system and different kind of static relationship between:
	- Classes.
	- Attributes.
	- Methods.
# Building Blocks
## Class
![[Pasted image 20221208130546.png|center]]
- Name on top.
- Attributes second with their types written after the colon.
- Method is last and the types they return are written after the colon.
- Before the names are access modifiers (class visibility notaion).
	- "+": Public.
	- "-": Private.
	- "#": Protected.
	- "~": Package Local.
- Parameters in methods can be described in terms of direction.
	- in: Indicates that Parameter values are passed in by the caller.
	- inout: Indicates that Parameter values are passed in by the caller and (possibly different) values passed out to the caller.
	- out: Indicates that Parameter values are passed out to the caller.
	- return: Indicates that Parameter values are passed as return values back to the caller.

![[Pasted image 20221208131427.png|center]]
## Perspectives
### Conceptual
- Conceptual perspective represents the concepts in the domain under study.
- A conceptual model should be drawn with little or no regard for the software that might implement it
### Specification
- Conceptual perspective represents the interfaces of the software, not the implementation.
- A conceptual model should be drawn with little or no regard for the software that might implement it
### Inplementation
- In this view, we really do have classes and we are laying the implementation bare.
- This is probably the perspective used most often, but in many ways the specification perspective is often a better one to take.
# Types of relationship
![[07-relationships-between-classes.webp|center]]
## 1.Association
- Relationship between classes.
- They are represented by a **solid line** between classes.
![[10-simple-association-example.webp|center]]
## 2.Inheritance (or Generalization)
- A generalization is a relationship between a more general classifier and a more specific classifier.
- The relationship is displayed as a **solid line** with a **hollow arrowhead** that points from the child element to the parent element.
![[08-inheritance-in-class-diagram.webp|center]]
## 3.Aggregation
- A special type of association.
- It represents a "part of" relationship.
- The relationship is displayed as a solid line with a unfilled diamond at the association end, which is connected to the class that represents the aggregate.
![[12-aggregation.webp|center]]
## 4.Composition
- A special type of aggregation where parts are destroyed when the whole is destroyed.
- Objects of Class2 live and die with Class1.
- Class2 cannot stand by itself.
- The relationship is displayed as a solid line with a filled diamond at the association end, which is connected to the class that represents the whole or composite.
![[13-composition.webp|center]]
## 5.Dependency
- An object of one class might use an object of another class in the code of a method. If the object is not stored in any field, then this is modeled as a dependency relationship.
- A special type of association.
- Exists between two classes if changes to the definition of one may cause changes to the other (but not the other way around).
- The relationship is displayed as a dashed line with an open arrow.
![[14-dependency.webp|center]]
## 6.Realization
- Realization is a relationship between the blueprint class and the object containing its respective implementation level details.
- In other words, you can understand this as the relationship between the interface and the implementing class.
![[16-realization.webp|center]]
### (Numbers at each end of the class association indicate the range of numbers of instances of classes allowed in the relationship)