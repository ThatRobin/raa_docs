# Stat Bar
[Power Types](../power_types.md)

Defines a stat bar for the player. Holds a persistent integer value between 0, and 20.

Type ID: `ra_additions:stat_bar`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `start_value` | [Int](../data_types/int.md) | _optional_ | The value of the resource when the player first gains this power. | 
 | `hud_render` | [Stat Bar Hud Render](../data_types/stat_bar_hud_render.md) | _optional_ | Specifies how and if the stat bar is displayed with a bar on the HUD. | 

### Example
```json
{
  "type": "ra_additions:stat_bar",
  "start_value": 20,
  "hud_render": {
    "should_render": true,
    "bar_index": 0,
    "side": "right",
    "sprite_location": "ra_additions:textures/gui/icons.png"
  },
  "icon": "minecraft:emerald",
  "name": "Mana Abilities",
  "description": "You can use mana with your magical staff to activate its powers."
}
```
This example is a stat bar, which creates a bar of the given texture that is already completely filled.
