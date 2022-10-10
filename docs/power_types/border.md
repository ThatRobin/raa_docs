# Border

[Power Type](../power_types.md).

Creates a border around the entity with this power. Only entities that fulfil the conditions may pass through it.

Type ID: `ra_additions:border`

### Fields

Field | Type | Default | Description
------|------|---------|------------
`border_texture` | [Identifier](../data_types/identifier.md) | `textures/misc/forcefield.png` | The texture used on the border.
`entity_condition` | [Entity Condition Type](https://origins.readthedocs.io/en/latest/types/entity_condition_types/) | _optional_ | If specified, if the entity colliding with the border fulfils the condition, it can walk through the border. 
`bientity_condition` | [Bi-Entity Condition Type](https://origins.readthedocs.io/en/latest/types/bientity_condition_types/) | _optional_ | If specified, if the entity colliding with the border, and the entity with this power fulfil the condition, the colliding entity can walk through the border. 
`red` | [float](../data_types/float.md) | `0.1254901961` | The red value of the border.
`green` | [float](../data_types/float.md) | `0.6274509804` | The green value of the border.
`blue` | [float](../data_types/float.md) | `1` | The blue value of the border.
`alpha` | [float](../data_types/float.md) | `0.5` | The alpha (transparency) value of the border.
`scroll_texture` | [boolean](../data_types/boolean.md) | `true` | Defines whether the border scrolls like the vanila border.
`size` | [float](../data_types/float.md) | `6` | The distance to one side of the border from the center.

### Example

```json
{
    "type": "ra_additions:border",
    "size": 12,
    "red": 1,
    "green": 1,
    "blue": 1,
    "alpha": 0.5,
    "scroll_texture": false,
    "border_texture": "minecraft:textures/block/dirt.png",
    "entity_condition": {
        "type": "origins:creative_flying"
    }
}
```
This power will create a border the entity will be able to walk through, but will be unable to fly through.