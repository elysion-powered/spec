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
