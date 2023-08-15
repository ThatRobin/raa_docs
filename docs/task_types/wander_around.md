# Wander Around
[Task Types](../task_types.md)

A goal that causes the entity to wander around.

Type ID: `ra_additions:wander_around`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `priority` | [Int](../data_types/int.md) | _optional_ | The priority of the goal, the lower, the more important. | 
 | `speed` | [Double](../data_types/double.md) | _optional_ | The speed it should wander at | 

### Example
```json
{
  "type": "ra_additions:wander_around",
  "priority": 0,
  "speed": 1
}
```

