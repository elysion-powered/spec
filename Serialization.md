Serialization
===

Any entity/node, scene or inherited classes do have serialization features which saves it as a JSON.

An example scene might look like this:

```javascript
{
  "name": "gameScene",
  "entities": [{
    "name": "player",
    "type": "sprite",
    "left": "10px",
    "top": "20px",
    "components": [{
      "name": "spritesheet",
      "defaultFrame": 0
    }]
  }, {
    "name": "enemy",
    "type": "sprite",
    "components": [{
      "name": "shootsBullets"
    }]
  }]
}
```
