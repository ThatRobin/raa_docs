# Flee Entity
[Task Types](../task_types.md)

A goal that causes the mob to run away from an entity.

Type ID: `ra_additions:flee_entity`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `priority` | [Int](../data_types/int.md) | _optional_ | The priority of the goal, the lower, the more important. | 
 | `distance` | [Float](../data_types/float.md) | _optional_ | The amount of blocks away the entity must be to be considered safe. | 
 | `slow_speed` | [Double](../data_types/double.md) | _optional_ | The slower speed it should flee at. | 
 | `fast_speed` | [Double](../data_types/double.md) | _optional_ | The faster speed it should flee at. | 
 | `bientity_condition` | [Bientity Condition](../bientity_condition_types.md) | _optional_ | A condition to check if it should run away from the target. | 

### Example
```json
{
  "type": "ra_additions:flee_entity",
  "priority": 0,
  "distance": 8,
  "slow_speed": 1.6,
  "fast_speed": 1.4,
  "bientity_condition": {
    "type": "apoli:target_condition",
    "condition": {
      "type": "apoli:entity_type",
      "entity_type": "minecraft:creeper"
    }
  }
}
```

