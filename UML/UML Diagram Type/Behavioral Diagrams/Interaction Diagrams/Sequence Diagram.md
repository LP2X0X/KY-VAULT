# About
- A sequence diagram is an interaction diagram that emphasizes the time-ordering of messages. It depicts the objects and classes involved in the scenario and the sequence of messages exchanged between the objects needed to carry out the functionality of the scenario.
# Sequence Diagram Notations
## Actor
- A type of role played by the instance that interacts with the subject.
- Actors represents roles played by users, external equipment, or other actors.
- Actor does not necessarily represent a specific physical entity, but simply a specific role of some entity.
- A person can play the role of several different actors, and an actor may be played by multiple different people.
## Object
- In the UML, an object in a sequence diagram is drawn as a rectangle containing the name of the object, underlined. An object can be named in one of three ways: the object name, the object name and its class, or just the class name (anonymous object).
## Lifeline
- Entities of participants in a collaboration (scenario) are written horizontally across the top of the diagram. A lifeline is represented by dashed vertical line drawn below each object. These indicate the existence of the object.
## Message
- Messages depict the invocation of operations are shown horizontally. 
- They are drawn from the sender to the receiver. Ordering is indicated by vertical position, with the first message shown at the top of the diagram, and the last message shown at the bottom. As a result, sequence numbers is optional.
- The line type and arrowhead type indicates the type of message being used:
1. A **synchronous message** (typically an operation call) is shown as a solid line with a filled arrowhead. It is a regular message call used for normal communication between sender and receiver.
![[02-lifelines-with-synchronous-message.png|center]]
2. A **return message** uses a dashed line with an open arrowhead.
![[03-lifelines-with-return-message.webp|center]]
3. An **asynchronous message** has a solid line with an open arrowhead. A signal is an asynchronous message that has no reply.
![[Pasted image 20221208204142.png|center]]
## Creation and Destruction Messages
- Participants do not necessarily live for the entire duration of a sequence diagram's interaction. Participants can be created and destroyed according to the messages that are being passed.
- A **constructor message** creates its receiver. The sender that already exist at the start of the interaction are placed at the top of the diagram. Targets that are created during the interaction by a constructor call are automatically placed further down the diagram.
![[Pasted image 20221208204221.png|center]]
- A **destructor message** destroys its receiver. There are other ways to indicate that a target is destroyed during an interaction. Only when a target's destruction is set to 'after destructor' do you have to use a destructor.
![[Pasted image 20221208204246.png|center]]
## Non instantaneous message
- Messages are often considered to be instantaneous, thus, the time it takes to arrive at the receiver is negligible. The messages are drawn as a horizontal arrow. 
- To indicate that it takes a certain while before the receiver actually receives a message, a **slanted arrow is used**.
![[Pasted image 20221208204309.png|center]]
## Focus of Control
- Focus of Control represents the period during which an element is performing an operation. The top and the bottom of the of the rectangle are aligned with the initiation and the completion time respectively
## Iteration notation
- **Iteration notation** represents a message is sent many times to multiple receiver objects, as would happen when you are iterating over a collection. You can show the basis of the iteration within brackets, such as *[for all order lines].
## Sequence Fragments
- In a UML sequence diagram, combined fragments let you show loops, branches, and other alternatives. A combined fragment consists of one or more interaction operands, and each of these encloses one or more messages, interaction uses, or combined fragments.
- A sequence fragment is represented as a box called a combined fragment, which encloses a portion of the interactions within a sequence diagram. The fragment operator (in the top left cornet) indicates the type of fragment. Fragment types include ref, assert, loop, break, alt, opt and neg, ref, sd.

| Operator | Meaning                                                                                                                                                                                     |
| -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| alt      | Alternative multiple fragments: only the one whose condition is true will execute.                                                                                                          |
| opt      | Optional: the fragment executes only if the supplied condition is true. Equivalent to an alt only with one trace.                                                                           |
| par      | **Parallel**: each fragment is run in parallel.                                                                                                                                             |
| loop     | **Loop**: the fragment may execute multiple times, and the guard indicates the basis of iteration.                                                                                          |
| critical | **Critical region**: the fragment can have only one thread executing it at once.                                                                                                            |
| neg      | **Negative**: the fragment shows an invalid interaction.                                                                                                                                    |
| ref      | **Reference**: refers to an interaction defined on another diagram.<br>The frame is drawn to cover the lifelines involved in the interaction. You can define parameters and a return value. |
| sd       | **Sequence diagram**: used to surround an entire sequence diagram.                                                                                                                          |
