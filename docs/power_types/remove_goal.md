# Remove Goal
[Power Types](../power_types.md)

The entity with this power will have any goals listed removed from itself.

Type ID: `ra_additions:remove_goal`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `goal` | [String](../data_types/string.md) | _optional_ | The goal to remove from the mob. | 
 | `goals` | [Array](../data_types/array.md) of [String](../data_types/string.md) | _optional_ | The goals to remove from the mob. | 

### Example
```json
{
  "type": "ra_additions:remove_goal",
  "goals": [
    "attack",
    "bow_attack"
  ],
  "example_pack": "This example will prevent a mob from doing standard attacks, and bow attacks."
}
```

