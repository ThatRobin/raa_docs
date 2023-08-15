# Boss Bar
[Power Types](../power_types.md)

Defines a boss bar for the player. Essentially identical to a [Resource Bar](https://origins.readthedocs.io/en/latest/types/power_types/resource/) but displays as a boss bar.

Type ID: `ra_additions:boss_bar`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `min` | [Int](../data_types/int.md) | _optional_ | The minimum value of the boss bar. | 
 | `max` | [Int](../data_types/int.md) | _optional_ | The maximum value of the boss bar. | 
 | `start_value` | [Int](../data_types/int.md) | _optional_ | The value of the boss bar when the entity first receives the power. If not set, this will be set to the value of the min integer field. | 
 | `hud_render` | [Boss Bar Hud Render](../data_types/boss_bar_hud_render.md) | _optional_ | Determines how the boss bar is visualized on the HUD. | 
 | `text` | [Text](../data_types/text.md) | _optional_ | The text displayed above the boss bar. | 
 | `min_action` | [Entity Action](../entity_action_types.md) | _optional_ | If specified, this action will be executed on the entity whenever the minimum value is reached. | 
 | `max_action` | [Entity Action](../entity_action_types.md) | _optional_ | If specified, this action will be executed on the entity whenever the maximum value is reached. | 

### Example
```json
{
  "type": "ra_additions:boss_bar",
  "min": 0,
  "max": 20,
  "start_value": 20,
  "hud_render": {
    "should_render": true,
    "bar_index": 0,
    "sprite_location": "textures/gui/bars.png"
  },
  "icon": "minecraft:emerald",
  "name": "Mana Abilities",
  "description": "You can use mana with your magical staff to activate its powers."
}
```
This example is a boss bar, which creates a bar that is already completely filled.
