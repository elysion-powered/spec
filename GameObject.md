GameObject
---

An game object is an object (which may or may not have a graphical representation) which can be added to a scene
or other game objects.

Similar to a scene it has to implement two methods:
* Rendering the entity (While this is always visible/accessible, it will be not be called on non-graphical entities)
* Updating the entity

Additionally, these types of objects can be added to any game object:
* Behaviour [0..*]
* DataModel [0..*]

Game objects can communicate with each other (through a parent object which is either a scene or a game object), and can either trigger custom events or pre-defined events.
