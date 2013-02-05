Elysion Specification
===

Scene Management
---

Definition of a scene
---

A scene is an encapsuled visual reprensentation of entities. For example in a game the main menu will be a scene,
whereas the options screen is a different scene as well as each level of the game will be most likely a different
scene.

The scene has to provide following functions:
* Rendering the graphical components of a scene
* Updating the behaviour of each component

Definition of a scene director
---

The scene director is similar to a scene, but allows one or more scenes to be registered without being able for
entities to be added to the scene director itself.
