# Tempt
[Task Types](../task_types.md)

A goal that causes the entity to be tempted.

Type ID: `ra_additions:tempt`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `priority` | [Int](../data_types/int.md) | _optional_ | The priority of the goal, the lower, the more important. | 
 | `speed` | [Double](../data_types/double.md) | _optional_ | The speed it should follow at | 
 | `can_be_scared` | [Boolean](../data_types/boolean.md) | _optional_ | Can the entity be scared off? | 
 | `bientity_condition` | [Bientity Condition](../bientity_condition_types.md) | _optional_ | A condition to check if it should follow the target. | 

### Example
```json
{
  "type": "ra_additions:tempt",
  "priority": 0,
  "speed": 1.2,
  "can_be_scared": true,
  "bientity_condition": {
    "type": "apoli:target_condition",
    "condition": {
      "type": "apoli:entity_type",
      "entity_type": "minecraft:creeper"
    }
  }
}
```

