# About
- A use case describes how a user uses a system to accomplish a particular goal.
- A use case is a list of actions or event steps typically defining the interactions between a role of an actor and a system to achieve a goal.
- A use case is made up of a set of possible sequences of interactions between systems and users that defines the features to be implemented and the resolution of any errors that may be encountered.
- A use case (or set of use cases) has these characteristics:
	- Organizes functional requirements.
	- Models the goals of system/actor (user) interactions.
	- Describes one main flow of events (main scenarios) and possibly other exceptional flows (alternatives), also called paths or user scenarios.
# Use Case Diagram Notations
![[02-use-case-diagram-notations.webp|center]]
## Actor
- Actors are usually individuals involved with the system defined according to their roles. The actor can be a human or other external system.
## Use Case
- A use case describes how actors uses a system to accomplish a particular goal. 
- Use cases are typically initiated by a user to fulfill goals describing the activities and variants involved in attaining the goal.
## Relationship
- The relationships between and among the actors and the use cases.
## System Boundary
- The system boundary defines the system of interest in relation to the world around it.
# Structuring Use Cases
## << include >> Use Case
- The time to use the << include >> relationship is after you have completed the first cut description of all your main Use Cases. You can now look at the Use Cases and identify common sequences of user-system interaction.
![[04-include-use-case-example.png|center]]
## << extend >> Use Case
- An extending use case is, effectively, an alternate course of the base use case. 
- The << extend >> use case accomplishes this by conceptually inserting additional action sequences into the base use-case sequence.
![[05-extend-use-case-example.png|center]]