# Revenge
[Task Types](../task_types.md)

A goal that causes the entity to seek revenge on the entity that hits it.

Type ID: `ra_additions:revenge`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `priority` | [Int](../data_types/int.md) | _optional_ | The priority of the goal, the lower, the more important. | 
 | `bientity_condition` | [Bientity Condition](../bientity_condition_types.md) | _optional_ | A condition to check if it should attack the target. | 

### Example
```json
{
  "type": "ra_additions:revenge",
  "priority": 0
}
```

