# Escape Danger
[Task Types](../task_types.md)

A goal that causes the mob to run away when hit.

Type ID: `ra_additions:escape_danger`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `priority` | [Int](../data_types/int.md) | _optional_ | The priority of the goal, the lower, the more important. | 
 | `speed` | [Double](../data_types/double.md) | _optional_ | The speed it should escape at | 
 | `bientity_condition` | [Bientity Condition](../bientity_condition_types.md) | _optional_ | A condition to check if it should run away from the target. | 

### Example
```json
{
  "type": "ra_additions:escape_danger",
  "priority": 0,
  "speed": 1.25,
  "bientity_condition": {
    "type": "apoli:target_condition",
    "condition": {
      "type": "apoli:entity_type",
      "entity_type": "minecraft:creeper"
    }
  }
}
```

