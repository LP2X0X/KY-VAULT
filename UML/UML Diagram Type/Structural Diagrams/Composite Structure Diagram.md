# About
- A composite structure diagram is a UML structural diagram that contains classes, interfaces, packages, and their relationships, and that provides a logical view of all, or part of a software system. It shows the internal structure (including parts and connectors) of a structured classifier or collaboration.
- A composite structure diagram performs a similar role to a class diagram, but allows you to go into further detail in describing the internal structure of multiple classes and showing the interactions between them. You can graphically represent inner classes and parts and show associations both between and within classes.
# Purpose of Composite Structure Diagram
- Composite Structure Diagrams allow the users to "Peek Inside" an object to see exactly what it is composed of.
- The internal actions of a class, including the relationships of nested classes, can be detailed.
- Objects are shown to be defined as a composition of other classified objects.
# Basic Concepts of Composite Structure Diagram
## Collaboration
- A collaboration describes a structure of collaborating parts (roles). A collaboration is attached to an operation or a classifier through a Collaboration Use. You use a collaboration when you want to define only the roles and connections that are required to accomplish a specific goal of the collaboration.
- For example, the goal of a collaboration can be to define the roles or the components of a classifier. By isolating the primary roles, a collaboration simplifes the structure and clarifies behavior in a model.
## Parts
- A part is a diagram element that represents a set of one or more instances that a containing structured classifier owns. A part describes the role of an instance in a classifier. You can create parts in the structure compartment of a classifier, and in several UML diagrams such as composite structure, class, object, component, deployment, and package diagrams.
## Port
- A port defines the interaction point between a classifier instance and its environment or between the behavior of the classifier and its internal parts.
## Interface
- Composite Structure diagram supports the ball-and-socket notation for the provided and required interfaces. Interfaces can be shown or hidden in the diagram as needed.
## Connector
- A line that represents a relationship in a model. When you model the internal structure of a classifier, you can use a connector to indicate a link between two or more instances of a part or a port. The connector defines the relationship between the objects or instances that are bound to roles in the same structured classifier and it identifies the communication between those roles. The product automatically specifies the kind of connector to create.
