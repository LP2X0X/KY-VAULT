# About
- Timing diagrams are UML interaction diagrams used to show interactions when a primary purpose of the diagram is to reason about time. 
- Timing diagrams focus on conditions changing within and among lifelines along a linear time axis. 
- Timing Diagrams describe behavior of both individual classifiers and interactions of classifiers, focusing attention on time of occurrence of events causing changes in the modeled conditions of the Lifelines.
# Basic Concepts of Timing Diagrams
## Lifeline
- A lifeline in a Timing diagram forms a rectangular space within the content area of a frame. 
- Lifeline is a named element which represents an individual participant in the interaction. It is typically aligned horizontally to read from left to right.
![[Pasted image 20221208210314.png|center]]
- Multiple lifelines may be stacked within the same frame to model the interaction between them.
![[Pasted image 20221208210330.png|center]]
## State Timeline in Timing Diagram
- A state or condition timeline represents the set of valid states and time. The states are stacked on the left margin of the lifeline from top to bottom.
- The cause of the change, as is the case in a state or sequence diagram, is the receipt of a message, an event that causes a change, a condition within the system, or even just the passage of time.
![[Pasted image 20221208210512.png|center]]
## Multiple Compartments
- It is possible to stack several life lines of different objects in the same timing diagram. One life line above the other. 
- Messages sent from one object to another can be depicted using simple arrows. The start and the end points of each arrow indicate when each message was sent and when it was received.
![[07-multiple-lifelines-in-timing-frame.png|center]]
## State Lifeline
- A state lifeline shows the change of state of an item over time. The X-axis displays elapsed time in whatever units are chosen while the Y-axis is labelled with a given list of states.
![[Pasted image 20221208210601.png|center]]
## Value Lifeline
- A value lifeline shows the change of value of an item over time. The X-axis displays elapsed time in whatever units are chosen, the same as for the state lifeline. 
- The value is shown between the pair of horizontal lines which crosses over at each change in value.
![[Pasted image 20221208210641.png|center]]
## Timeline and Constraints
- We can use the length of a timeline to indicate how long the object remains in a particular state by reading it from left to right. To associate time measurements, you show tick marks online the bottom part of the frame.
- You can use relative time marks in constraints to indicate that a message must be received within a specified amount of time.
![[Pasted image 20221208210712.png|center]]
## State and Value Lifeline Side-by-Side
- State and Value Lifelines can be put one after the other in any combination. Messages can be passed from one lifeline to another. 
- Each state or value transition can have a defined event, a time constraint which indicates when an event must occur, and a duration constraint which indicates how long a state or value must be in effect for.