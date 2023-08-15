# Value
[Power Types](../power_types.md)

Defines a value for the player. Essentially identical to a [Resource Bar](https://origins.readthedocs.io/en/latest/types/power_types/resource/) but displays as number in a string.

Type ID: `ra_additions:value`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `min` | [Int](../data_types/int.md) | _optional_ | The minimum value of the power. | 
 | `max` | [Int](../data_types/int.md) | _optional_ | The maximum value of the power. | 
 | `anchor` | null | _optional_ | The part of the screen that can be used as the center point | 
 | `x` | [Int](../data_types/int.md) | _optional_ | The X co-ordinate that the string will appear at. | 
 | `y` | [Int](../data_types/int.md) | _optional_ | The Y co-ordinate that the string will appear at. | 
 | `value_key` | [String](../data_types/string.md) | _optional_ | The string that will contain the value | 
 | `start_value` | [Int](../data_types/int.md) | _optional_ | The value of the power when the entity first receives it. If not set, this will be set to the value of the min integer field. | 

### Example
```json
{
  "type": "ra_additions:value",
  "x": 70,
  "y": 70,
  "min": 5,
  "max": 10,
  "value_key": "You have %s value"
}
```
This example is a value, which creates a string of text that says `you have %s value` where %s is the internal value of the power.
