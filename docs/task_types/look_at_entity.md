# Look At Entity
[Task Types](../task_types.md)

A goal that causes the mob to look at the closest entity.

Type ID: `ra_additions:look_at_entity`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `priority` | [Int](../data_types/int.md) | _optional_ | The priority of the goal, the lower, the more important. | 
 | `range` | [Float](../data_types/float.md) | _optional_ | The range in which the target can be looked at. | 
 | `bientity_condition` | [Bientity Condition](../bientity_condition_types.md) | _optional_ | A condition to check if it should look at the target. | 

### Example
```json
{
  "type": "ra_additions:melee_attack",
  "priority": 0,
  "range": 6,
  "bientity_condition": {
    "type": "apoli:target_condition",
    "condition": {
      "type": "apoli:entity_type",
      "entity_type": "minecraft:creeper"
    }
  }
}
```

