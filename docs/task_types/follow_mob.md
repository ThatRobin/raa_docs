# Follow Mob
[Task Types](../task_types.md)

A goal that causes the mob to follow an entity.

Type ID: `ra_additions:follow_mob`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `priority` | [Int](../data_types/int.md) | _optional_ | The priority of the goal, the lower, the more important. | 
 | `speed` | [Double](../data_types/double.md) | _optional_ | The speed it should follow at | 
 | `can_be_scared` | [Boolean](../data_types/boolean.md) | _optional_ | Can the entity be scared? | 
 | `bientity_condition` | [Bientity Condition](../bientity_condition_types.md) | _optional_ | A condition to check if it should follow the target. | 

### Example
```json
{
  "type": "ra_additions:follow_mob",
  "priority": 0,
  "speed": 1,
  "can_be_scared": false,
  "bientity_condition": {
    "type": "apoli:target_condition",
    "condition": {
      "type": "apoli:entity_type",
      "entity_type": "minecraft:creeper"
    }
  }
}
```

