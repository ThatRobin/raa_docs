# Cat Sit On Block
[Task Types](../task_types.md)

A goal that allows a cat to sit on a block.

Type ID: `ra_additions:cat_sit_on_block`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `priority` | [Int](../data_types/int.md) | _optional_ | The priority of the goal, the lower, the more important. | 
 | `speed` | [Double](../data_types/double.md) | _optional_ | The speed that the cat will move to the block at. | 

### Example
```json
{
  "type": "ra_additions:cat_sit_on_block",
  "priority": 0,
  "speed": 1
}
```

