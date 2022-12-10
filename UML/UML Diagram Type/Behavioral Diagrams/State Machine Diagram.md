# About
- State Machine Diagrams (or sometimes referred to as state diagram, state machine or state chart) show the different states of an entity. 
- State machine diagrams can also show how an entity responds to various events by changing from one state to another.
- State machine diagram is a diagram used to model the dynamic nature of a system. 
- State machine diagram typically are used to describe state-dependent behavior for an object. 
- An object responds differently to the same event depending on what state it is in.
# Characteristics of State Machine Notations
- A state occupies an interval of time.
- A state is often associated with an abstraction of attribute values of an entity satisfying some condition(s).
- An entity changes its state not only as a direct consequence of the current input, but it is also dependent on some past history of its inputs.
# Basic Concepts of State Machine Diagram
## State
- A state is an abstraction of the attribute values and links of an object. Sets of values are grouped together into a state according to properties that affect the gross behavior of the object.
![[02-state-notations.webp|center]]
### Characteristics
- State represent the conditions of objects at certain points in time.
- Objects (or Systems) can be viewed as moving from state to state.
- A point in the lifecycle of a model element that satisfies some condition, where some particular action is being performed or where some event is waited.
## Initial and Final States
- The initial state of a state machine diagram, known as an initial pseudo-state, is indicated with a solid circle. A transition from this state will show the first real state
- The final state of a state machine diagram is shown as concentric circles. An open loop state machine represents an object that may terminate before the system terminates, while a closed loop state machine diagram does not have a final state; if it is the case, then the object lives until the entire system terminates.
![[Pasted image 20221208193351.png|center]]
## Events
- An event signature is described as Event-name (comma-separated-parameter-list). Events appear in the internal transition compartment of a state or on a transition between states. 
- An event may be one of four types:
	- Signal event - corresponding to the arrival of an asynchronous message or signal.
	- Call event - corresponding to the arrival of a procedural call to an operation.
	- Time event - a time event occurs after a specified time has elapsed.
	- Change event - a change event occurs whenever a specified condition is met.
### Characteristics
- Represents incidents that cause objects to transition from one state to another.
- Internal or External Events trigger some activity that changes the state of the system and of some of its parts.
- Events pass information, which is elaborated by Objects operations. Objects realize Events
- Design involves examining events in a state machine diagram and considering how those events will be supported by system objects.
## Transition
- Transition lines depict the movement from one state to another.
- Multiple transitions occur either when different events result in a state terminating or when there are guard conditions on the transitions
- A transition without an event and action is known as automatic transitions
- Transitions between states occur as follows:
	- An element is in a source state.
	- An event occurs.
	- An action is performed.
	- The element enters a target state.
## Actions and Activity

- Action is an executable atomic computation, which includes operation calls, the creation or destruction of another object, or the sending of a signal to an object. An action is associated with transitions and during which an action is not interruptible - e.g., entry, exit.
- Activity is associated with states, which is a non-atomic or ongoing computation. Activity may run to completion or continue indefinitely. An Activity will be terminated by an event that causes a transition from the state in which the activity is defined.
### Characteristics
- States can trigger actions.
- States can have a second compartment that contains actions or activities performed while an entity is in a given state.
- An action is an atomic execution and therefore completes without interruption.
- Five triggers for actions: On Entry, Do, On Event, On Exit, and Include.
- An activity captures complex behavior that may run for a long duration - An activity may be interrupted by events, in which case it does not complete occur when an object arrives in a state.
## Entry and Exit Actions
- Entry and Exit actions specified in the state. It must be true for every entry / exit occurrence. If not, then you must use actions on the individual transition arcs:
	- **Entry Action** executed on entry into state with the **notation: Entry / action**
	- **Exit Action** executed on exit from state with the **notation: Exit / action**
## Substates
- A simple state is one which has no substructure. 
- A state which has substates (nested states) is called a composite state.
## History States
- History states allow the state machine to re-enter the last substate that was active prior to leaving the composite state.
![[Pasted image 20221208194332.png|center]]
## Concurrent State
- States in state machine diagrams can be nested. Related states can be grouped together into a single composite state.
![[Pasted image 20221208200804.png|center]]