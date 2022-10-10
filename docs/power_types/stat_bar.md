# Stat Bar

[Power Type](../power_types.md).

Defines a stat bar for the player. Holds a persistent integer value between 0, and 20.

Type ID: `ra_additions:stat_bar`

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`hud_render` | [Stat Bar Hud Render](../data_types/stat_bar_hud_render.md) | | Specifies how and if the stat bar is displayed with a bar on the HUD.
`start_value` | [Integer](../data_types/integer.md) | `20` | The value of the resource when the player first gains this power.

### Example
```json
{
    "type": "ra_additions:stat_bar",
    "start_value": 20,
    "hud_render": {
        "should_render": true,
        "bar_index": 0,
        "side": "right",
        "sprite_location": "kunzite_pack:textures/gui/icons.png"
    },
    "icon": "minecraft:emerald",
    "name": "Mana Abilities",
    "description": "You can use mana with your magical staff to activate its powers."
}
```

This example is a stat bar, which creates a bar of the given texture that is already completely filled.
