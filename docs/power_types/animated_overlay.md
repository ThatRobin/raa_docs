# Animated Overlay
[Power Types](../power_types.md)

Lets you have a texture overlay onto the entity that you can have change over time.

Type ID: `ra_additions:animated_overlay`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `interval` | [Int](../data_types/int.md) | _optional_ | The amount of ticks before swapping to the next texture. | 
 | `texture_location` | [Identifier](../data_types/identifier.md) | _optional_ | The texture location to use for the overlay. | 
 | `texture_locations` | [Array](../data_types/array.md) of [Identifier](../data_types/identifier.md) | _optional_ | The texture locations to use for the overlay. | 

### Example
```json
{
  "type": "ra_additions:animated_overlay",
  "texture_locations": [
    "minecraft:textures/entity/zombie/drowned_outer_layer.png",
    "minecraft:textures/entity/zombie/zombie.png",
    "minecraft:textures/entity/zombie/husk.png"
  ],
  "interval": 10
}
```
This example will make the player look like they are wearing some diamond armour.
