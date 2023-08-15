# Swim
[Task Types](../task_types.md)

A goal that causes the entity to swim in water.

Type ID: `ra_additions:swim`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `priority` | [Int](../data_types/int.md) | _optional_ | The priority of the goal, the lower, the more important. | 
 | `fluid_type` | null | _optional_ | The type of fluid it should be able to swim in. | 

### Example
```json
{
  "type": "ra_additions:revenge",
  "priority": 0,
  "fluid_type": "water"
}
```

