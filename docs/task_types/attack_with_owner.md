# Attack With Owner
[Task Types](../task_types.md)

A goal that causes its mob to target whoever its owner attacks.

Type ID: `ra_additions:attack_with_owner`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `priority` | [Int](../data_types/int.md) | _optional_ | The priority of the goal, the lower, the more important. | 
 | `attacking_condition` | [Bientity Condition](../bientity_condition_types.md) | _optional_ | A condition to see if it can attack its target. | 
 | `owner_condition` | [Bientity Condition](../bientity_condition_types.md) | _optional_ | A condition to see if it can attack with the owner. | 

### Example
```json
{
  "type": "ra_additions:attack_with_owner",
  "priority": 0,
  "attacking_condition": {
    "type": "apoli:target_condition",
    "condition": {
      "type": "apoli:entity_type",
      "entity_type": "minecraft:creeper"
    }
  },
  "owner_condition": {
    "type": "apoli:target_condition",
    "condition": {
      "type": "apoli:sneaking"
    }
  }
}
```

