# Add Goal

[Power Type](../power_types.md).

Adds a custom goal (from `data/{namespace}/goals/`) to the entity with this power.

Type ID: `ra_additions:add_goal`

!!! note

    The addition of custom goals is not yet complete, and is not documented.

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`goal` | [Identifier](../data_types/identifier.md) | _optional_ | The goal to add to the mob.
`goals` | [Array](../data_types/array.md) of [Identifiers](../data_types/identifier.md) | _optional_ | The goals to add to the mob.


### Example
```json
{
    "type": "ra_additions:add_goal",
    "goal": "example:stuff"
}
```
This example will apply the example:stuff (`data/example/goals/stuff.json`) mob goal to the entity with the power.
```json
{
    "type": "ra_additions:tempt",
    "priority": 0,
    "speed": 1.2,
    "can_be_scared": false,
    "bientity_condition": {
        "type": "origins:target_condition",
        "condition": {
            "type": "origins:equipped_item",
            "equipment_slot": "mainhand",
            "item_condition": {
                "type": "origins:ingredient",
                "ingredient": {
                    "item": "minecraft:diamond"
                }
            }
        }
    }
}
```
This being the contents of the example:stuff (`data/example/goals/stuff.json`) goal.