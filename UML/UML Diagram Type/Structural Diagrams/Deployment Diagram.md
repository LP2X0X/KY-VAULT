# About
- Deployment diagrams is used to visualize the static aspect of these physical nodes and their relationships and to specify their details for construction.
- Deployment diagrams are one of the two kinds of diagrams used in modeling the physical aspects of an object-oriented system.
- They can be use to plan System Architecture.
# Deployment Diagram Notations
## 1.Component
- A component is a grouping of classes that work together closely. 
- Components can be classified by their type. Some components exist only at compile time, some exist only at link time, some exist only at run time; and some exist at more than one time.
## 2.Node
- A node is a run-time physical object that represents a computational resource, generally having memory and processing capability. 
- You can model node types and node instances. You may model the component instances that run or live on a node by drawing them within the node. 
- You may model which nodes communicate with one another using the Connection relationship line.
![[02-deployment-diagram-node.png|center]]
## 3.Dependency
- A dependency indicates that one model element (source) depends on another model element (target), such that a change to the target element may require a change to the source element in the dependency. 
- In a deployment diagram, you can use the dependency relationship to show the capability of a node type to support a component type. You may also use the relationship to show the dependency between component types.
## 4.Connection
- A connection depicts the communication path used by the hardware to communicate usually indicates the method i.e. TCP/IP.
![[03-deployment-diagram-connection.png|center]]
## 4.Artifact
- Artifacts represent concrete elements in the physical world that are the result of a development process. 
- Examples of artifacts are executable files, libraries, archives, database schemas, configuration files, etc.
![[04-deployment-diagram-node-and-artifacts.png|center]]