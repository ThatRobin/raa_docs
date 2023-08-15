# Animal Mate
[Task Types](../task_types.md)

A goal that causes its mob to find a mate to breed with.

Type ID: `ra_additions:animal_mate`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `priority` | [Int](../data_types/int.md) | _optional_ | The priority of the goal, the lower, the more important. | 
 | `speed` | [Double](../data_types/double.md) | _optional_ | the speed that the entity will move to its mate. | 

### Example
```json
{
  "type": "ra_additions:animal_mate",
  "priority": 0,
  "chance": 1
}
```

