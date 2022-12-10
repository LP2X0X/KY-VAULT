# About
- Activity diagram is essentially an advanced version of flow chart that modeling the flow from one activity to another activity.
# When to use
- Identify candidate use cases, through the examination of business workflows.
- Identify pre- and post-conditions (the context) for use cases.
- Model workflows between/within use cases.
- Model complex workflows in operations on objects.
- Model in detail complex activities in a high level activity Diagram.
![[02-basic-activity-diagram.webp|center]]


| Notation Description                                                                                                                                   | UML Notation                                                |
| ------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------- |
| Activity: Is used to represent a set of actions                                                                                                        | ![[09-activity-diagram-notation-activity 1.webp\|center]]   |
| Action: A task to be performed                                                                                                                         | ![[Pasted image 20221208161938.png\|center]]                |
| Control Flow: Show the sequence of execution                                                                                                           | ![[11-activity-diagram-notation-control-flow.webp\|center]] |
| Object Flow: Show the flow of an object from one <br>activity (or action) to another activity (or action)                                              | ![[Pasted image 20221208164515.png\|center]]                | 
| Initial Node: Portrays the beginning of a set of <br>action or activities                                                                              | ![[Pasted image 20221208164521.png\|center]]                |
| Activities Final Node: Stop all control flows and <br>object flows in an activity (or action)                                                          | ![[Pasted image 20221208164526.png\|center]]                |
| Object Node: Represent an object that is connected to<br> a set of Object Flows                                                                        | ![[Pasted image 20221208164529.png\|center]]                |
| Decision Node: Represent a test condition to ensure that <br>the control flow or object flow only goes down one path                                   | ![[Pasted image 20221208164533.png\|center]]                |
| Merge Node: Bring back together different decision paths that<br> were created using a decision-node                                                   | ![[Pasted image 20221208164543.png\|center]]                |
| Fork Node: Split behavior into a set of parallel or concurrent<br> flows of activities (or actions)                                                    | ![[Pasted image 20221208164546.png\|center]]                |
| Join Node: Bring back together a set of parallel or concurrent<br> flows of activities (or actions)                                                    | ![[Pasted image 20221208164554.png\|center]]                |
| Swimlane and Partition: A way to group activities performed by<br> the same actor on an activity <br>diagram or to group activities in a single thread | ![[Pasted image 20221208164557.png\|center]]                |



