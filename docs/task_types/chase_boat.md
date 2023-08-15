# Chase Boat
[Task Types](../task_types.md)

A goal that causes its mob to chase boats.

Type ID: `ra_additions:chase_boat`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `priority` | [Int](../data_types/int.md) | _optional_ | The priority of the goal, the lower, the more important. | 
 | `bientity_condition` | [Bientity Condition](../bientity_condition_types.md) | _optional_ | A condition to see if it can chase the boat. | 

### Example
```json
{
  "type": "ra_additions:chase_boat",
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

