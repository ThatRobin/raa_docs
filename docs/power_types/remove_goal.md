# Remove Goal

[Power Type](../power_types.md).

The entity with this power will have any goals listed removed from itself.

Type ID: `ra_additions:remove_goal`

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`goal` | [Vanilla Goal](../data_types/vanilla_goal.md) | _optional_ | The goal to add to the mob.
`goals` | [Array]() of [Vanilla Goal](../data_types/vanilla_goal.md) | _optional_ | The goals to add to the mob.


### Example
```json
{
    "type": "ra_additions:remove_goal",
    "goals": [
        "attack",
        "bow attack"
    ]
}
```
This example will prevent a mob from doing standard attacks, and bow attacks.