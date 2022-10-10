# Stat Bar Hud Render

[Data Type](../data_types.md).

An [Object](object.md) used to define how a stat bar should be rendered.

### Fields:

Field  | Type | Default | Description
-------|------|---------|-------------
`should_render` | [Boolean](boolean.md) | `true` | Whether the bar should be visible or not.
`sprite_location` | [Identifier](identifier.md) | `"ra_additions:textures/gui/resource_bar.png"` | The path to the file in the assets which contains what the bar looks like. The base mod doesn't include any bars, but you can create your own using Resource Packs.
`bar_index` | [Integer](integer.md) | `0` | The indexed position of the bar on the sprite to use. Please note that indexes start at 0.
`condition` | [Entity Condition](https://origins.readthedocs.io/en/latest/types/entity_condition_types/) | _optional_ | If set (and `should_render` is true), the bar will only display when the entity with the power fulfills this condition.
`side` | [String](string.md) | `"right"` | Determines which side of the players HUD the bar appears on. Can be `"left"` or `"right"`.

### Examples:

```json
"hud_render": {
    "should_render": true,
    "bar_index": 2,
    "side": "right"
}
```

This definition shows the stat bar as the Redstone bar.
<br>

```json
"hud_render": {
    "should_render": true,
    "bar_index": 0,
    "side": "right",
    "sprite_location": "example_pack:textures/gui/icons.png"
}
```

This definition shows the stat bar as the example packs first icon, being a blue orb.
