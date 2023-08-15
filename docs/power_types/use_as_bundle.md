# Use As Bundle
[Power Types](../power_types.md)

Allows an item to be used like a bundle, with a customizable capacity.

Type ID: `ra_additions:use_as_bundle`
### Fields
 | Field | Type | Default | Description | 
|---|---|---|---|
 | `max_amount` | [Int](../data_types/int.md) | _optional_ | the amount of items you can store in the bundle. | 
 | `item_condition` | [Item Condition](../item_condition_types.md) | _optional_ | Items that fulfil this condition, will be bundle-like. | 

### Example
```json
{
  "type": "ra_additions:use_as_bundle",
  "hold_amount": 64,
  "item_condition": {
    "type": "apoli:nbt",
    "nbt": "{isBundle:1b}"
  }
}
```
This example makes it so that any item with the nbt data `{isBundle:1b}` is able to be used as a bundle.
