# Boss Bar Hud Render

[Data Type](../data_types.md).

An [Object](object.md) used to define how a boss bar should be rendered.

### Fields:

Field  | Type | Default | Description
-------|------|---------|-------------
`should_render` | [Boolean](boolean.md) | `true` | Whether the bar should be visible or not.
`bar_index` | [Integer](integer.md) | `0` | The indexed position of the bar on the sprite to use. Please note that indexes start at 0.
`priority` | [Integer](integer.md) | `0` | The order in which the bar appears on the screen.
`overlays` | [Array](array.md) of [Boss Bar Hud Overlay](boss_bar_hud_overlay.md) | _optional_ | The overlays you can display on the boss bar.
`sprite_location` | [Identifier](identifier.md) | `"textures/gui/bars.png"` | The path to the file in the assets which contains what the bar looks like.
`condition` | [Entity Condition](https://origins.readthedocs.io/en/latest/types/entity_condition_types/) | _optional_ | If set (and `should_render` is true), the bar will only display when the entity with the power fulfills this condition.
`inverted` | [Boolean](boolean.md) | `false` | Determines whether greater values increment or decrement the bar.

### Examples:

```json
"hud_render": {
    "should_render": true,
    "bar_index": 2
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
