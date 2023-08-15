# Melee Attack
[Task Types](../task_types.md)

A goal that causes the mob to use melee attacks against the target.

Type ID: `ra_additions:melee_attack`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `priority` | [Int](../data_types/int.md) | _optional_ | The priority of the goal, the lower, the more important. | 
 | `bientity_condition` | [Bientity Condition](../bientity_condition_types.md) | _optional_ | A condition to check if it should attack the target. | 

### Example
```json
{
  "type": "ra_additions:melee_attack",
  "priority": 0,
  "bientity_condition": {
    "type": "apoli:target_condition",
    "condition": {
      "type": "apoli:entity_type",
      "entity_type": "minecraft:creeper"
    }
  }
}
```

