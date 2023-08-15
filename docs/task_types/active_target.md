# Active Target
[Task Types](../task_types.md)

A target goal that finds a target by entity class when the goal starts.

Type ID: `ra_additions:active_target`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `priority` | [Int](../data_types/int.md) | _optional_ | The priority of the goal, the lower, the more important. | 
 | `reciprocal_chance` | [Int](../data_types/int.md) | _optional_ | The chance to search for a target per tick. | 
 | `check_visibility` | [Boolean](../data_types/boolean.md) | _optional_ | Should it check if the target is visible or not? | 
 | `check_can_navigate` | [Boolean](../data_types/boolean.md) | _optional_ | Should it check if it can navigate to the target. | 
 | `bientity_condition` | [Bientity Condition](../bientity_condition_types.md) | _optional_ | which entities should be able to be targeted. | 

### Example
```json
{
  "type": "ra_additions:active_target",
  "priority": 0,
  "reciprocal_chance": 10,
  "check_visibility": true,
  "check_can_navigate": false,
  "bientity_condition": {
    "type": "apoli:attacker"
  }
}
```

