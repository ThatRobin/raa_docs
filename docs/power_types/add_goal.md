# Add Goal
[Power Types](../power_types.md)

Adds a custom goal (from `data/{namespace}/goals/`) to the entity with this power.

Type ID: `ra_additions:add_goal`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `goal` | [Identifier](../data_types/identifier.md) | _optional_ | The goal to add to the mob. | 
 | `goals` | [Array](../data_types/array.md) of [Identifier](../data_types/identifier.md) | _optional_ | The goals to add to the mob. | 

### Example
```json
{
  "type": "ra_additions:add_goal",
  "goal": "ra_additions:revenge_example"
}
```
This example will apply the `example:stuff` mob goal to the entity with the power.
