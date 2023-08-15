# Attack
[Task Types](../task_types.md)

A goal that causes its mob to follow and attack its selected target.

Type ID: `ra_additions:attack`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `priority` | [Int](../data_types/int.md) | _optional_ | The priority of the goal, the lower, the more important. | 
 | `bientity_condition` | [Bientity Condition](../bientity_condition_types.md) | _optional_ | A condition to see if it can attack its target. | 

### Example
```json
{
  "type": "ra_additions:attack",
  "priority": 0,
  "bientity_condition": {
    "type": "apoli:attacker"
  }
}
```

