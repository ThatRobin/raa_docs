# Creeper Ignite
[Task Types](../task_types.md)

A goal that allows creepers to ignite

Type ID: `ra_additions:creeper_ignite`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `priority` | [Int](../data_types/int.md) | _optional_ | The priority of the goal, the lower, the more important. | 
 | `bientity_condition` | [Bientity Condition](../bientity_condition_types.md) | _optional_ | A condition to see if the target should cause the creeper to ignite | 

### Example
```json
{
  "type": "ra_additions:creeper_ignite",
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

