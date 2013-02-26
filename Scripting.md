Scripting
===

While implementing scripting into Elysion is entirely optional, it is definitely recommended.
The recommended scripting language is JavaScript (or any language that compiles to JavaScript) to keep a level of 
interoperability between similar Elysion game engines.

A game object for example will look like this:

```javascript
(function(gameOject) {
  // Code goes here
})(this)
```

The same would be this in CoffeeScript:

```coffeescript
do (gameObject = @) ->
  # Code goes here
```
