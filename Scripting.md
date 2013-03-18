Scripting
===

While implementing scripting into Elysion is entirely optional, it is definitely recommended.
The recommended scripting language is JavaScript (or any language that compiles to JavaScript) to keep a level of 
interoperability between Elysion-like game engines.

A game object script can be attached to any Elysion game object. A very basic example would look like this:

```javascript
(function(gameOject) {
  // Code goes here
})(this);
```

The same would be this in CoffeeScript:

```coffeescript
do (gameObject = @) ->
  # Code goes here
```

Any properties and methods can be used from the game object.
```coffeescript
do (gameObject = @) ->

  @on 'update', (dt) ->
    gameObject.rotate 3.0 * dt
```

This example will cause the game object to rotate each frame.


Additionally to game objects, scenes can be scripted as well. It should provide the flexibility to write a whole game
in the scripting engine, but developers are not forced to do so at all. This also allows for the whole codebase to be
written in a single language and target all Elysion-like engines with all the platforms they support.
