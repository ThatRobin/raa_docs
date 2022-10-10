# Boss Bar

[Power Type](../power_types.md).

Defines a boss bar for the player. Essentially identical to a [Resource Bar]() but displays as a boss bar.

Type ID: `ra_additions:boss_bar`

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`text` | [String](../data_types/text_component.md) | _optional_ | The text displayed above the boss bar.
`min` | [Integer](../data_types/integer.md) | *manditory* | The minimum value of the boss bar.
`max` | [Integer](../data_types/integer.md) | *manditory* | The maximum value of the boss bar.
`hud_render` | [Custom Hud Render](../data_types/hud_render.md) | _optional_ | Determines how the boss bar is visualized on the HUD.
`start_value` | [Integer](../data_types/integer.md) | _optional_ | The value of the boss bar when the entity first receives the power. If not set, this will be set to the value of the `min` integer field.
`min_action` | [Entity Action Type](../entity_action_types.md) | _optional_ | If specified, this action will be executed on the entity whenever the minimum value is reached.
`max_action` | [Entity Action Type](../entity_action_types.md) | _optional_ | If specified, this action will be executed on the entity whenever the maximum value is reached.

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
