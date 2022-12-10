# About
- A communication diagram is an extension of object diagram that shows the objects along with the messages that travel from one to another.
# Purpose of Communication Diagram
- Model message passing between objects or roles that deliver the functionalities of use cases and operations.
- Model mechanisms within the architectural design of the system.
- Capture interactions that show the passed messages between objects and roles within the collaboration scenario.
- Model alternative scenarios within use cases or operations that involve the collaboration of different objects and interactions.
- Support the identification of objects (hence classes), and their attributes (parameters of message) and operations (messages) that participate in use cases.
# Communication Diagram Elements
- **Objects** participating in a collaboration come in two flavors: supplier and client.
	- **Supplier objects** are the objects that supply the method that is being called, and therefore receive the message.
	- **Client objects** call methods on supplier objects, and therefore send messages.

## Links
- The connecting lines drawn between objects in a communication diagram are links.
- These links are what set communication diagrams apart from sequence diagrams. They enable you to see the relationships between objects.
- Each link represents a relationship between objects and symbolizes the ability of objects to send messages to each other.
- If an object sends messages to itself, the link carrying these messages is represented as a loop icon. This loop can be seen on both the UI object and the Transaction object.
## Messages 
- Messages in communication diagrams are shown as arrows pointing from the Client object to the Supplier object. Typically, messages represent a client invoking an operation on a supplier object. 
- They can be modeled along with the objects in the following manner:
	- Message icons have one or more messages associated with them.
	- Messages are composed of message text prefixed by a sequence number.
	- This sequence number indicates the time-ordering of the message.
![[06-communication-diagram-elements.png|center]]